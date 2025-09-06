# Enhanced Service Dashboard

A powerful web-based dashboard for analyzing service ticket data with interactive charts and visualizations. This dashboard helps you understand patterns in your service requests, track performance metrics, and make data-driven decisions.

## Features

- **Multi-format Support**: Upload CSV, TXT, or Excel (.xlsx) files
- **Interactive Charts**: 11 different chart types for comprehensive data analysis
- **Dark Theme**: Modern, easy-on-the-eyes interface
- **Responsive Design**: Works on desktop and mobile devices
- **Real-time Processing**: Instant chart generation from uploaded data

## Chart Types

The dashboard generates the following visualizations:

1. **Ticket Status** - Distribution of ticket statuses
2. **Priority Distribution** - Breakdown by priority levels
3. **Item Type Distribution** - Analysis by ticket types
4. **Requestor Site Distribution** - Geographic/site-based analysis
5. **Deadline Compliance** - Breached vs. Compliant tickets
6. **Average Ticket Duration** - Time analysis in days
7. **Weekly Closed Tickets** - Weekly performance trends
8. **Monthly Closed Tickets** - Monthly performance trends
9. **Closed Tickets by Location** - Location-based completion analysis
10. **Open Ticket Extended** - Extension tracking
11. **Ticket Nature by Description** - Description-based categorization

## How to Use

### Step 1: Prepare Your Data
The dashboard is flexible and will work with various column names. Here are the expected columns (with alternative names that will be automatically detected):

**Required Columns (at least one of each category):**
- **Status**: `Status (Service Today)`, `Status`, `Ticket Status`
- **Priority**: `Priority`, `Priority Level`, `Urgency`
- **Type**: `Item type`, `Type`, `Category`, `Ticket Type`
- **Location**: `Requestor Site  `, `Requestor Site`, `Site`, `Location`
- **Workgroup**: `To workgroup  `, `To workgroup`, `Workgroup`, `Team`, `Department`

**Optional Columns (for enhanced analytics):**
- **Dates**: `Deadline`, `Due Date`, `Target Date`
- **Timestamps**: `Modified`, `Created`, `Date`, `Timestamp`
- **Descriptions**: `Description`, `Summary`, `Details`, `Notes`
- **Extensions**: `Revised_Deadline`, `Revised Deadline`, `New Deadline`

**Note**: The dashboard will work with minimal data (just Status, Priority, Type) and will show warnings for missing optional columns while still providing useful analytics.

### Step 2: Upload Your File
1. Open the dashboard by opening `index.html` in your web browser
2. Click "Choose File" or drag and drop your data file
3. Supported formats: `.csv`, `.txt`, `.xlsx`
4. The dashboard will automatically process your data

### Step 3: Analyze the Results
- Charts will appear automatically after file upload
- Each chart provides insights into different aspects of your service data
- Use the charts to identify trends, bottlenecks, and improvement opportunities

## File Format Requirements

### CSV/TXT Files
- Must have headers in the first row
- Use comma-separated values
- Ensure proper date formatting for `Deadline` and `Modified` columns

### Excel Files
- First sheet will be used for data processing
- Headers should be in the first row
- Date columns should be properly formatted

## Data Processing Features

- **Automatic Date Calculations**: Calculates ticket duration and deadline compliance
- **Smart Categorization**: Groups data by various dimensions
- **Week/Month Analysis**: Automatically extracts temporal patterns
- **Extension Tracking**: Identifies tickets with revised deadlines
- **Description Analysis**: Categorizes tickets by description keywords

## Browser Compatibility

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Any modern browser with JavaScript enabled

## Technical Requirements

- No server required - runs entirely in the browser
- Requires internet connection for loading external libraries:
  - Bootstrap 5.3.0 (CSS framework)
  - Chart.js (charting library)
  - PapaParse (CSV parsing)
  - SheetJS (Excel file processing)

## Troubleshooting

### Common Issues

**Charts not appearing:**
- Check that your file has the correct column headers
- Ensure your data file is not empty
- Verify the file format is supported (.csv, .txt, .xlsx)

**Data not processing correctly:**
- Check that you have at least basic columns (Status, Priority, Type)
- The dashboard will automatically detect alternative column names
- Ensure date columns are properly formatted if using date-based analytics
- Verify CSV files use comma separators
- Missing optional columns will show warnings but won't prevent processing

**File upload fails:**
- Check file size (very large files may cause issues)
- Ensure file extension is correct
- Try a different browser if problems persist

## Privacy & Security

- All data processing happens locally in your browser
- No data is sent to external servers
- Your files remain on your device
- Safe for sensitive or confidential data

## Getting Started

1. Download or clone this repository
2. Open `index.html` in your web browser
3. Prepare your service ticket data file
4. Upload and start analyzing!

## Support

For issues or questions:
1. Check the troubleshooting section above
2. Verify your data format matches the requirements
3. Ensure you're using a supported browser

---

*This dashboard is designed to help you gain insights from your service ticket data quickly and efficiently.*