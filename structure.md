assettrack/                      ← put in C:\xampp\htdocs\
├── front-end/
│   ├── index.html               page shell, loads the CSS and JS
│   ├── css/
│   │   ├── tokens.css           colors, fonts, dark mode
│   │   ├── base.css             layout, sidebar, cards, tables, forms
│   │   └── print.css            QR label printing
│   ├── js/
│   │   ├── utils.js             esc(), badge(), opt(), toast()
│   │   ├── store.js             data layer (localStorage now, fetch() to the API later)
│   │   ├── qr.js                qrSvg() and link()
│   │   ├── app.js               router, render(), sidebar shell
│   │   └── views/
│   │       ├── login.js
│   │       ├── dashboard.js
│   │       ├── assets.js        list, add asset, asset detail
│   │       ├── reports.js       admin report list and status changes
│   │       ├── labels.js        printable QR sheet
│   │       ├── report-page.js   public scan page (QR opens this)
│   │       └── user.js          "Report an issue" and "My reports"
│   └── lib/
│       └── qrcode.min.js        local copy so it works offline
│
├── back-end/
│   ├── config/
│   │   └── db.php               MySQL connection settings
│   ├── api/
│   │   ├── auth.php             login, logout, session check
│   │   ├── assets.php           list, add, update assets
│   │   └── reports.php          submit and update reports
│   ├── database/
│   │   └── schema.sql           users, assets, reports tables and sample data
│   └── uploads/                 report photos
│
└── README.md                    setup steps for the group


(Structure Made by Henrich G. Angeles)