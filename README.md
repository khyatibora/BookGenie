# 📚 BookGenie

**BookGenie** is an AI-powered book recommendation assistant designed to help users explore books across genres and moods. It features a clean, interactive web interface and integrates IBM Watson Assistant for chatbot-based recommendations.

---

## 🌟 Features

* 🔍 Get book suggestions by **genre**, **mood**, or **author**
* 🤖 Chatbot-powered interaction via IBM Watson Assistant
* 🎨 Beautiful front-end UI with genre-based book cards
* 📚 Supports genres like:

  * Horror 🦹
  * Thriller 🔍
  * Romance 💌
  * Inspirational 💡

---

## 🚀 Live Demo

🔗 [View Demo](https://khyatibora.github.io/BookGenie) *(Add GitHub Pages link if hosted)*

---

## 🖼 Homepage Preview

![BookGenie Screenshot](https://user-images.githubusercontent.com/your-image-path.png)
*A clean layout showing book cards and Watson chatbot integration.*

---

## 🛠️ Technologies Used

* **HTML5** + **CSS3**
* **JavaScript** (minimal for chat integration)
* **IBM Watson Assistant** – [Watson Integration](https://cloud.ibm.com/assistant/)
* 📷 Background & book cover images from Unsplash & Amazon

---

## 📦 Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/khyatibora/BookGenie.git
   cd BookGenie
   ```

2. Open `index.html` in your browser to explore the site locally.

---

## 🤖 Watson Chat Integration

The chatbot is embedded via IBM Watson Assistant script. Integration IDs can be found in the `index.html` file:

```html
<script>
  window.watsonAssistantChatOptions = {
    integrationID: "YOUR-INTEGRATION-ID",
    region: "YOUR-REGION",
    serviceInstanceID: "YOUR-SERVICE-ID",
    onLoad: async (instance) => { await instance.render(); }
  };
  setTimeout(() => {
    const t = document.createElement('script');
    t.src = "https://web-chat.global.assistant.watson.appdomain.cloud/versions/latest/WatsonAssistantChatEntry.js";
    document.head.appendChild(t);
  });
</script>
```

> 🚩 **Note**: Replace integration ID with your own if deploying independently.

---

## 📚 Sample Conversations

* **User**: "Can you recommend a romantic book?"
  **Assistant**: "Sure! Try *Me Before You* by Jojo Moyes."

* **User**: "What thriller books do you have?"
  **Assistant**: "You might enjoy *Gone Girl* by Gillian Flynn."

---

## ✨ Future Enhancements

* 📖 Dynamic book database/API integration
* 🎯 Mood-based suggestions with filters
* 📱 Mobile responsive chatbot improvements

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

Made with ❤️ by [@khyatibora](https://github.com/khyatibora)
