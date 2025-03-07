# React-Datepicker-Day-1-of-Exploring-JS-Libraries
Yesterday, I needed a date picker library and came across react-datepicker. As I explored it, I found it to be quite interesting and user-friendly. So, I decided to write a quick overview for anyone looking for a basic understanding of how it works.

# 📅 React Date Picker Overview  

`react-datepicker` is a popular and highly customizable date picker component for React applications. This guide provides a basic overview of its installation, usage, and key features.  

## ✅ Installation  

Install the package using **npm** or **yarn**:  

```sh
npm install react-datepicker --save
```
or

```sh
yarn add react-datepicker
```

## 📌 Date-Fns (Optional but Recommended)
For enhanced date formatting, install `date-fns`:

```sh
npm install date-fns
```
or 

```sh
yarn add date-fns
```

## 🚀 How to Use React Date Picker?
After successful installation, import react-datepicker in your component:

```sh

import DatePicker from "react-datepicker";
import "react-datepicker/dist/react-datepicker.css";

```
🗒️ Note: Make sure to import the CSS file to apply default styles.

##⚒️ Basic Usage
The simplest way to use react-datepicker is as follows:

```sh
import React, { useState } from "react";
import DatePicker from "react-datepicker";
import "react-datepicker/dist/react-datepicker.css";

const MyDatePicker = () => {
  const [startDate, setStartDate] = useState(new Date());

  return <DatePicker selected={startDate} onChange={(date) => setStartDate(date)} />;
};

export default MyDatePicker;

```

👓 Expected Output:
A simple date picker where users can select a date.

![Alt Text](https://raw.githubusercontent.com/YourUsername/YourRepo/main/assets/images/your-image.png)
