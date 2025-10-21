
# Syncfusion Vue Pivot Table – Getting Started Sample

This sample demonstrates how to **integrate the Syncfusion Pivot Table (PivotView) component** into a **Vue 3 application using Vue CLI**. It showcases key features such as field list, grouping bar, calculated fields, and custom formatting.

## 📖 Overview

The Syncfusion Pivot Table (PivotView) is a powerful component for summarizing and analyzing large datasets. This sample helps you get started with the Pivot Table in a Vue 3 project and demonstrates how to:

- Bind a JSON data source.
- Configure rows, columns, values, and filters.
- Set custom height and width for the Pivot Table.
- Enable dynamic field manipulation using the Field List.
- Use the Grouping Bar for drag-and-drop field arrangement.
- Add calculated fields using basic arithmetic operations.

## 🚀 Getting Started

### Prerequisites

Before running this sample, ensure you have the following installed:

- [Node.js](https://nodejs.org/)
- [Vue CLI](https://cli.vuejs.org/)

### Installation Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/SyncfusionExamples/vue3-pivottable-getting-started
   cd vue3-pivottable-getting-started
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Run the application:**
   ```bash
   npm run serve
   ```

4. **Open in browser:**
   Navigate to `http://localhost:8080` to view the Pivot Table in action.

## 🔧 Key Features Demonstrated

1. **JSON Data Binding:**
   The Pivot Table is populated using a local JSON array containing sales data.

2. **Field Configuration:**
   - **Rows:** `Country`
   - **Columns:** `Year`
   - **Values:** `Amount`, `Total` (calculated field)

3. **Calculated Fields:**
   A new field `Total` is added using the formula:
   ```js
   calculatedFieldSettings: [{ name: 'Total', formula: '"Sum(Amount)"+"Sum(Sold)"' }]
   ```

4. **Field List:**
   Allows users to dynamically add, remove, and rearrange fields at runtime.

5. **Grouping Bar:**
   Enables drag-and-drop interaction for customizing the Pivot Table layout.

6. **Formatting:**
   Currency formatting is applied to the `Amount` field:
   ```js
   formatSettings: [{ name: 'Amount', format: 'C1' }]
   ```

## 📂 Project Structure

```
vue3-pivottable-getting-started/
├─ public/
│  ├─ favicon.ico
│  └─ index.html
├─ src/
│  ├─ assets/
│  │  └─ logo.png
│  ├─ App.vue
│  └─ main.js
├─ README.md
├─ package.json
└─ babel.config.js
```

## 📚 Learn More

- [Syncfusion Vue Pivot Table Documentation](https://ej2.syncfusion.com/vue/documentation/pivotview/getting-started/)
- [Syncfusion Vue Pivot Table Demos](https://ej2.syncfusion.com/vue/demos/#/material3/pivot-table/overview)

## 💬 Support

For questions or feedback, visit the [Syncfusion Support Portal](https://support.syncfusion.com) or [Community Forums](https://www.syncfusion.com/forums).

## 📜 License

This is a commercial product and requires a valid Syncfusion license.  
[View License Terms](https://www.syncfusion.com/license/studio/22.2.5/syncfusion_essential_studio_eula.pdf)
