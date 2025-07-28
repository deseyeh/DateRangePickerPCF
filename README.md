# 📅 Date Range Picker PCF

## 🧭 Introduction

The **Date Range Picker PCF** is a custom control built with React and Fluent UI that enables users to select a start and end date using a range picker UI in Power Apps. The control offers quick preset ranges, visual styling, and validation.

 ---


## 🚀 Example
![Sample Image](https://github.com/deseyeh/DateRangePickerPCF/blob/main/_example.png)



## 🛠️ Installation and Usage

1. Import the control into your PCF solution.
2. Bind the `startDate` and `endDate` properties to date fields.
3. Optionally configure appearance, range presets, and footer.

---

## 🧩 Configuration

The control is configured through PCF manifest properties. No external services are used.

> [!NOTE]
> ## For Some reason, the control should be configured in the Classic.

---
<img width="232" alt="image" src="https://github.com/user-attachments/assets/d0db9a84-19c0-4b9b-b909-f27dcdc5f001" />

 
![Sample Image](https://github.com/deseyeh/DateRangePickerPCF/blob/main/datarangeConfig.PNG) 



---

## 🎨 Appearance Options

Control the visual style using `dateVariant` and `dateSize`:

### `dateVariant`

* `outlined` (default)
* `filled`
* `borderless`
* `underlined`

### `dateSize`

* `small`
* `middle` (default)
* `large`

  ### `show Range Presets`

*Yes or No

### `Preset Ranges`
This will only show if show Range Presets is Yes. If the String is not a valid JSON, it will default to the default Presets.
Only add custom preset if you want something defrent from the Preset range.

[   { "label": "Last 7 Days", "value": -7 },    { "label": "Last 14 Days", "value": -14 }, 
         { "label": "Last 30 Days", "value": -30 }, 
          { "label": "Last 90 Days", "value": -90 } 
  ]

## 📅 Default Preset Ranges

| Preset Label   | Description                             |
| -------------- | --------------------------------------- |
| `Last 7 Days`  | Sets start date to 7 days before today  |
| `Last 14 Days` | Sets start date to 14 days before today |
| `Last 30 Days` | Sets start date to 30 days before today |
| `Last 90 Days` | Sets start date to 90 days before today |
| `To Days`      | Sets both start and end date to today   |
| `Next 7 Days`  | Sets end date to 7 days after today     |
| `Next 14 Days` | Sets end date to 14 days after today    |
| `Next 30 Days` | Sets end date to 30 days after today    |
| `Next 90 Days` | Sets end date to 90 days after today    |
---

## 🧾 Properties

| Property       | Type              | Usage  | Description                                         |
| -------------- | ----------------- | ------ | --------------------------------------------------- |
| `startDate`    | Date/Text/Decimal | bound  | Required start date                                 |
| `endDate`      | Date/Text/Decimal | bound  | Required end date                                   |
| `show Range Presets` | TwoOptions        | input  | Show/hide preset options (default: true)            |
| `Preset Ranges - Array of objects` | Text        | input  | Array of Objects ( lable and Value           |
| `extraFooter`  | Text              | input  | Optional footer message                             |
| `dateVariant`  | Enum              | input  | Control appearance variant                          |
| `dateSize`     | Enum              | input  | Control size                                        |
| `dateOutput`   | Object            | output | Output object with date info                        |
| `DataSchema`   | Text              | input  | Hidden property used for output schema registration |

---




---


 

