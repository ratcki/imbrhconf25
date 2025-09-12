# Internal Medicine Conference 2025 - Buriram Hospital

A responsive website for the Internal Medicine Department's annual academic conference at Buriram Hospital, Thailand. The conference theme is "Harmony of Care: Bridging General Care to Specialty Medicine".

## 🌟 Features

- Responsive design with Tailwind CSS
- Event countdown timer
- Registration form integration
- Mobile-friendly navigation
- Interactive FAQ section
- Location map integration

## 🛠️ Tech Stack

- HTML5
- CSS3 (with Tailwind CSS)
- JavaScript (Vanilla)
- Google Fonts (Sarabun)
- Google Maps Embed API

## 📁 Project Structure

```
imbrhconf25/
│
├── index.html          # Main HTML file with embedded styles and scripts
│
└── public/           # Static assets
    ├── Logo.png      # Conference logo
    ├── cover.png     # Social media cover image
    ├── favicon.ico   # Website favicon
    └── agenda.json   # Dynamic agenda data
```

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/ratcki/imbrhconf25.git
   ```

2. Open `index.html` in your web browser or use a local development server.

3. To customize the registration form, edit the `REGISTER_URL` constant in the `<script>` section of `index.html`.

## ⚙️ Configuration

The following settings can be configured in the `<script>` section of `index.html`:

- `REGISTER_URL`: URL for the registration form
- `EVENT_START_ISO`: Event start date/time in ISO 8601 format
- `EVENT_END_ISO`: Event end date/time in ISO 8601 format
- `LOGO_SRC`: Path to the conference logo image

Additional agenda items can be configured in `public/agenda.json`.

## 📅 Event Details

- **Dates**: November 6-7, 2025
- **Venue**: Buriram Hospital Conference Hall
- **Target Audience**: Healthcare professionals from community hospitals in Buriram province
- **Registration**: Free admission

## 🤝 Contributing

Feel free to submit issues and enhancement requests.

## 📝 License

This project is for internal use at Buriram Hospital. All rights reserved.