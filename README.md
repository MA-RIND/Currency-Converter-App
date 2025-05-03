
```markdown
# 💱 Currency Converter App

A fast and simple **React Native** currency converter app that helps users convert Indian Rupees (₹) into multiple international currencies in real time. This app is designed with usability and responsiveness in mind, using modern UI components and clean architecture.

---

## 🌟 Features

- 🔢 Convert INR to multiple foreign currencies instantly
- 🔎 Select from a list of currencies
- ⚠️ Form validation with real-time feedback using Snackbar
- 💡 Clean, intuitive UI with FlatList rendering
- ✅ Platform-compatible for Android and iOS

---

## 🧠 How It Works

1. User enters an amount in Indian Rupees (₹).
2. User taps on a target currency button (e.g., USD, EUR, etc.).
3. The app calculates and displays the converted amount.
4. The selected currency button is highlighted for visual feedback.
5. If the input is empty or invalid, a Snackbar message is shown.

---

## 🔧 Technologies Used

- **React Native**
- **TypeScript**
- `react-native-snackbar`
- Custom components (`CurrencyButton`)
- FlatList & Pressable components for responsive UI

---

## 📁 Project Structure

```

.
├── App.tsx                 # Main App component
├── components/
│   └── CurrencyButton.tsx  # Custom button component for currency
├── constants/
│   └── currencyByRupee.ts  # List of currency rates and metadata

````

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
````

### 2. Install Dependencies

```bash
npm install
```

### 3. Run the App

* For **Android**:

```bash
npx react-native run-android
```

* For **iOS**:

```bash
npx react-native run-ios
```

---

## 🖼️ Sample UI

> Add screenshots or a short demo here to show off the app’s interface!

---

## 🔐 Input Validation & Error Handling

Handled using **Snackbar** for a non-intrusive user experience. Triggers include:

* Empty input field
* Non-numeric values

Example:

```ts
Snackbar.show({
  text: "Enter a value to convert",
  backgroundColor: "#EA7773",
  textColor: "#000000"
});
```

---

## ⚙️ Conversion Logic

```ts
const convertedValue = inputAmount * targetValue.value;
const result = `${targetValue.symbol} ${convertedValue.toFixed(2)}`;
```

---

## ✨ Custom Styling

Styled using `StyleSheet` for optimized performance. Example:

```ts
selected: {
  backgroundColor: '#ffeaa7',
},
```

The selected currency is visually highlighted to indicate the current target currency.

---

## 👨‍💻 Developer

Crafted with care by [**MA-RIND**](https://github.com/MA-RIND)

