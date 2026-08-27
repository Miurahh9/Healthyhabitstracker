# Daily Check – Private Habit Tracker

**A simple, zero-server habit tracker.** Ask yourself yes/no questions once a day, track your answers over time, and stay accountable to yourself.

All your data stays on your device. No servers, no accounts, no tracking.

## 🎯 What It Does

- **Daily questions**: Answer a set of yes/no questions every day. Default questions come with it, but you can customize them fully.
- **Weekly check-ins**: On your chosen day of the week (Sunday by default), you can answer an additional set of weekly questions to look back on your week.
- **Visual calendar**: See your yes/no answers at a glance in a 7-day or 30-day calendar view.
- **Stats per question**: Dive into individual questions to see your yes/no streak and completion rate.
- **Data export & import**: Download your full history as a .txt file, or email it to yourself. Import it back anytime to restore or migrate your data.
- **Calendar reminders**: Generate a .ics file to add a daily reminder to your calendar app.
- **Bilingual**: Works in English and Nederlands (Dutch). Language preference is saved.

## 🔒 Privacy

- **100% local storage**: Every question, answer, and setting is saved in your browser's localStorage. Nothing leaves your device.
- **No internet connection required**: Works fully offline. You can use it on a plane, in the subway, or anywhere.
- **No accounts or login**: Just open it and start. No email, no password, no data collected.

## 🚀 How to Use

### Online
Open [Daily Check on GitHub Pages](https://miurahh9.github.io/Healthyhabitstracker/) (or wherever it's hosted).

### Locally
1. Clone this repo or download `index.html`.
2. Open `index.html` in your browser.
3. That's it—start answering questions.

## 📋 Quick Start

1. **First run**: You'll see three default daily questions and two default weekly questions.
2. **Answer questions**: Tap **YES** or **NO** to log your answer for the day.
3. **Skip for now**: If you're not ready to answer, tap "Skip this for now"—you'll see it again later the same day.
4. **Customize**: Go to **MENU** → **List Questions** to edit, add, or delete questions. Changes take effect immediately.
5. **View history**: Go to **MENU** → **Calendar** to see your answers over the past 7 or 30 days. Click on a question to see its own stats.
6. **Back up your data**: Go to **MENU** → **Export Data** to download a file or email yourself a copy.

## ⚙️ Configuration

Edit the top of the script in `index.html` to customize:

```javascript
const defaultQuestions = [
    "Did you drink enough water today?",
    "Did you take your medication today?",
    "Did you get enough sleep last night?"
];

const defaultWeeklyQuestions = [
    "Did you exercise at least 3 times this week?",
    "Did you eat balanced meals this week?"
];

const weeklyTriggerDay = 0;  // 0 = Sunday, 6 = Saturday
const contactEmail = "rewindingsunflower@proton.me";
```

These settings only affect the **first run**. Once you've added or edited questions, they're fully in your control.

## 🌐 Browser Support

Works on all modern browsers (Chrome, Firefox, Safari, Edge). Requires localStorage support and JavaScript enabled.

Best experience on mobile—designed for portrait orientation.

## 📝 Data Format

Your data is stored in localStorage with simple keys:

- `my_questions`: JSON array of all questions `[{id, text, freq}, ...]`
- `log_YYYY-MM-DD_<question-id>`: YES or NO answer for that day
- `app_lang`: Your language preference (en or nl)

You can inspect this in your browser's Developer Tools → Application → Local Storage.

## 🎨 Features

- **Responsive design**: Works on phones, tablets, and desktops.
- **Accessible**: Full keyboard navigation, screen reader support, ARIA labels.
- **Dark theme**: Easy on the eyes, especially at night.
- **No dependencies**: Pure HTML, CSS, and JavaScript—one file, nothing to install.
- **Auto-save**: Your answers are saved instantly. No manual sync needed.

## ✨ Made with AI, Non-Profit

This app was created with the help of AI. It's free, open-source, and made with care.

## 🤝 Feedback

Found a bug? Have a suggestion? Open the **Contact** menu inside the app to send feedback.

## 📄 License

Open-source. Use, fork, and modify as you like.

---

**Happy habit tracking!** 🎉
