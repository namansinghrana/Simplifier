
# Simplifier - AI Text Summarizer
<img width="1000" alt="image" src="https://github.com/user-attachments/assets/8016b677-e126-4ca9-9d38-b9e7871859e4">
Simplifier is a lightweight web app that quickly summarizes text using Hugging Face's NLP models. Built with HTML, CSS, and JavaScript, it provides an easy-to-use interface for generating concise summaries of lengthy content.

## Features

- **Instant Summaries**: Summarize any text with one click.
- **Clean, Simple UI**: Easy-to-navigate layout for quick usage.
- **Powered by Hugging Face**: Uses Hugging Face API for high-quality NLP summarization.

## Demo

Try it out: [👨🏻‍💻](https://ai-text-summarizer03.netlify.app/)


## How It Works

1. **Input Text**: Paste or type the text you want to summarize.
2. **Click "Summarize"**: The app sends your text to Hugging Face’s API to generate a summary.
3. **Get Results**: The summarized text will display within seconds.

## Setup

To use Simplifier locally:

1. **Clone the Repository**:
```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
```

2. **Add Your Hugging Face API Token**:
   - Open `summarize.js` and add your Hugging Face access token:
```javascript
      let config = {
    method: 'post',
    maxBodyLength: Infinity,
    url: 'https://api-inference.huggingface.co/models/facebook/bart-large-cnn',
    headers: {
      'Content-Type': 'application/json',
      'Authorization': 'Bearer ' +  process.env['ACCESS_TOKEN'] // Add Your token here
    },
    data: data
  };

```

3. **Open `index.html` in a Browser**.

## Technologies Used

- **Frontend**: HTML, CSS, JavaScript
- **API**: Hugging Face Transformers (using access token for summarization)

## License

This project is licensed under the MIT License.

---
## Contact

If you have any questions or want to contribute, feel free to reach out to me on [LinkedIn](https://www.linkedin.com/in/naman-singh-rana-a54842319) or via [Email](mailto:namanr738@gmail.com).

---

Enjoy faster reading with Simplifier!
