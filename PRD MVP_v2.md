# **Product Requirements Document: VizMarkdown MVP (GUI Version)**

Version: 1.1 (MVP)  
Status: Approved for MVP Development

### **1\. Introduction & Vision**

* **1.1. Vision Statement:** To provide the fastest and most intuitive way for anyone to create and share beautiful, embeddable charts.  
* **1.2. Product Overview:** VizMarkdown is a client-side tool that allows users to build and customize charts using a simple graphical interface. It provides an instant live preview and generates embed codes for web or email, making it effortless to add professional-looking visualizations to any content without writing code.

### **2\. The Problem**

* **2.1. Problem Statement:** Creating simple, embeddable charts for websites, blogs, or emails is often cumbersome. Existing tools can be overly complex for simple tasks, while coding charts from scratch requires technical knowledge that many users lack.  
* **2.2. How We Solve It:** Our product solves this by offering a single-page web application where a user can build a chart using intuitive form controls (like dropdowns, text boxes, and sliders). The tool provides immediate visual feedback and then generates the necessary embed codes.

### **3\. Target Audience & User Persona**

* **3.1. Target Market:** The initial target market includes content creators, bloggers, students, marketers, and developers who need to quickly create and embed simple data visualizations.  
* **3.2. User Persona:**  
  * **"Chris the Content Creator"**  
    * **Role:** Blogger for a tech website.  
    * **Goals:** Quickly add simple, polished charts to articles to make them more engaging. Find a tool that is faster than a spreadsheet program and more intuitive than a complex charting library.  
    * **Frustrations:** Spends too much time creating simple graphics. Wants more control over the look and feel of charts without having to learn code.

### **4\. Goals & Success Metrics**

* **4.1. Business Goals:**  
  * **Primary Goal: Idea Validation.** To validate that users desire a fast, GUI-based method for creating simple embeddable charts.  
  * Gather qualitative feedback on usability and the range of customization options from at least 20 initial testers.  
* **4.2. Product Goals & KPIs:**  
  * **Usage Rate:** 50% of unique visitors successfully generate at least one chart.  
  * **Satisfaction:** Collect direct user feedback to identify pain points and desired features.  
  * **Feature Discovery:** Track which chart types and customization options are most frequently used.

### **5\. Features & Functionality (MVP)**

* **5.1. Core Feature: Graphical Chart Builder**  
  * **Description:** A control panel with a series of intuitive UI elements that allow users to define and customize their chart.  
  * **User Story:** "As Chris, I want to use simple form controls to build my chart so I can easily see all my options and create a professional-looking visualization without guesswork."  
  * **Acceptance Criteria (Input Controls):**  
    1. **Type of Chart:** A dropdown list with the options: bar, line, pie, donut, and area.  
    2. **Chart Title:** A text box for the chart's title.  
    3. **Labels:** A text box to input comma-separated labels for the chart's data points (e.g., "Jan, Feb, Mar").  
    4. **Values:** A text area to input comma-separated data series. Each line represents a new series (e.g., "Series A, 10, 20, 30").  
    5. **X and Y Axis Labels:** Text boxes for each axis label (only visible for applicable chart types like bar and line).  
    6. **Show Values on Chart:** A checkbox or toggle switch to make data values visible directly on the chart.  
    7. **Rounded Borders:** A slider (range 0-100) to control the border radius of bars (for bar charts).  
    8. **Space Between Bars:** A slider (range 0-1) to control the spacing between bars in a bar chart.  
    9. **Font Options:** A dropdown list for font selection (e.g., 'Inter', 'Roboto', 'Arial') and icons/buttons for **Bold** and *Italic* styles for chart text.  
    10. **Chart Colors:** Three color picker inputs: (a) Background Color for the chart area, (b) Fill Color for the primary data series, and (c) Border Color for the primary data series.  
* **5.2. Other Core Features (Unchanged):**  
  * **Live Chart Preview:** An area on the page that renders a preview of the chart, updating in real-time as the user changes the controls.  
  * **Embed Code Generation:** Two text areas providing HTML snippets for embedding the chart on a website (iFrame) or in an email (static image). Includes "Copy" buttons.  
  * **Simulated Dashboard & Persistence:** The ability to save chart configurations to the browser's localStorage and view them in a "Dashboard" view.

### **6\. Design & User Experience (UX)**

* **6.1. User Flow:** User lands on page \-\> Uses the control panel to define and style their chart \-\> Views the live preview update instantly \-\> Clicks "Generate Embeds" \-\> Copies embed code \-\> Optionally clicks "Save" \-\> Navigates to "Dashboard" to manage saved charts.  
* **6.2. Wireframes & Mockups:** \[Link to a design file showing a two-panel layout: a control panel on the left and the live chart preview on the right\].

### **7\. Technical Requirements**

* **7.1. Tech Stack:**  
  * **Core:** Vanilla JavaScript and HTML.  
  * **Styling:** Tailwind CSS (linked via CDN).  
  * **Charting:** Chart.js library (linked via CDN).  
  * **Database:** Browser localStorage for persistence simulation.  
  * **Hosting:** A static hosting provider (e.g., Netlify, Vercel, GitHub Pages).

### **8\. Assumptions, Constraints & Dependencies**

* **8.1. Assumptions:** Users will find a graphical interface more intuitive than a text-based syntax. Client-side storage is sufficient for MVP validation.  
* **8.2. Constraints:** The MVP must be built within a single HTML file to maintain simplicity. Color options will apply to the primary data series first, with future iterations handling multi-series colors.  
* **8.3. Dependencies:** The project relies on the public CDNs for Chart.js and Tailwind CSS being available.

### **9\. Go-to-Market Plan**

* *(Unchanged from previous version)*

### **10\. Open Questions**

* How should the UI handle colors for multiple data series in a simple way?  
* What other customization options (e.g., legend position, gridline visibility) are most critical for users?  
* Do users still have a need for a "quick-add" text input alongside the GUI?