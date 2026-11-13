# 🐾 PetPal — Pet Care & Services Website

<p align="center">
  A clean, modern, and user-friendly pet care website built with HTML5 and CSS3.
</p>

<p align="center">
  <a href="https://asifs-lab.github.io/petpal-project/">Live Demo</a> •
  <a href="https://github.com/asifs-lab/petpal-project">GitHub Repository</a>
</p>

---

## 📌 About The Project

**PetPal** is a modern pet care website designed to present professional care services for beloved pets. The website focuses on creating a welcoming digital experience where pet owners can explore essential pet care services through a clean layout and visually engaging design.

The project demonstrates front-end development skills, structured HTML markup, custom CSS styling, and the use of SVG graphics and icons.

## ✨ Key Features

- **Modern Navigation:** Clean navigation bar with Home, Service, Blog, and Contact links.
- **Hero Section:** An engaging introduction with a clear call-to-action.
- **Pet Care Services:** Dedicated service cards highlighting:
  - Pet Vaccination
  - Professional Pet Grooming
  - Veterinary Care
  - Teeth Cleaning
- **Call-to-Action Buttons:** Prominent buttons for scheduling and pricing sections.
- **Custom Graphics:** SVG illustrations and visual elements.
- **Icon Integration:** Font Awesome icons for interface elements.
- **Clean Layout:** Organized sections with a consistent visual presentation.

## 🛠️ Technology Stack

| Technology   | Purpose                                  |
| ------------ | ---------------------------------------- |
| HTML5        | Website structure and semantic markup    |
| CSS3         | Styling, layout, and visual presentation |
| Font Awesome | Icon integration                         |
| SVG          | Scalable graphics and illustrations      |

## 📁 Project Structure

```text
petpal-project/
│
├── css/
│   └── style.css
│
├── images/
│   ├── header/
│   │   └── nav/
│   ├── hero/
│   └── can_do/
│       └── logo/
│
├── index.html
└── README.md
```

## 🚀 Getting Started

Follow these instructions to set up the project on your local machine.

### Prerequisites

- A modern web browser
- Visual Studio Code (recommended)
- Live Server extension (optional)

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/asifs-lab/petpal-project.git
```

**2. Navigate to the project directory**

```bash
cd petpal-project
```

**3. Open the project in VS Code**

```bash
code .
```

**4. Run the project**

Open `index.html` in your browser or launch it using the Live Server extension.

## 🌍 Live Website

Explore the deployed project:

**[PetPal — Live Preview](https://asifs-lab.github.io/petpal-project/)**

## 🎯 Project Goals

- Practice semantic HTML5 structure.
- Improve CSS layout and styling skills.
- Develop a visually consistent website interface.
- Work with SVG assets and external icon libraries.
- Build practical front-end development experience.

## 👨‍💻 Author

**Asif's Lab**

Front-End Developer | Creative Web Designer

- GitHub: [@asifs-lab](https://github.com/asifs-lab)
- Project: [PetPal Website](https://github.com/asifs-lab/petpal-project)

---

## 📄 License

This project is created for educational and portfolio purposes.

---

<p align="center">
  Designed & Developed with ❤️ by <strong>Asif's Lab</strong>
</p>

/_ Gradient layer (gradient transition hoy na, tai opacity diye fade) _/
.specialContent .cardSection .card::before {
content: "";
position: absolute;
inset: 0;
z-index: -1;
border-radius: inherit;
background: linear-gradient(180deg, #ffc49b 0%, #ffa466 41%, #ff7f24 98%);
opacity: 0;
transition: opacity var(--dur-fade) var(--ease);
}

/_ ================= TEXT ================= _/
.specialContent .cardSection .card h2,
.specialContent .cardSection .card h1,
.specialContent .cardSection .card .para p {
transition: color var(--dur-text) var(--ease);
}

.specialContent .cardSection .card h2 {
font-family: "Manjari", sans-serif;
font-weight: 700;
font-size: 24px;
line-height: 36px;
letter-spacing: 0.01em;
margin-bottom: 54px;
color: #27233a;
}

.specialContent .cardSection .card h1 {
font-family: "Manjari", sans-serif;
font-weight: 700;
font-size: 90px;
line-height: 72px;
letter-spacing: 0.01em;
margin-bottom: 44px;
color: #ff9a55;
}

/_ $ ar /visit jodi span/pseudo hoy, tader o smooth color change _/
.specialContent .cardSection .card h1 \*,
.specialContent .cardSection .card h1::before,
.specialContent .cardSection .card h1::after {
transition:
color var(--dur-text) var(--ease),
background var(--dur-text) var(--ease),
border-color var(--dur-text) var(--ease);
}

.specialContent .cardSection .card .para {
display: flex;
flex-direction: column;
align-items: center;
gap: 30px;
margin-bottom: 56px;
}

.specialContent .cardSection .card .para p {
font-family: "Manjari", sans-serif;
font-weight: 700;
font-size: 24px;
line-height: 24px;
letter-spacing: 0.01em;
color: #3d394e;
opacity: 0.75;
}

/_ ================= BUTTON ================= _/
.specialContent .cardSection .card button {
position: relative;
isolation: isolate;
overflow: hidden;
padding: 18px 67px;
border: none;
border-radius: 50px;
font-family: "Manjari", sans-serif;
font-weight: 700;
font-size: 24px;
color: #ffffff;
cursor: pointer;
background: linear-gradient(90deg, #ff7f24 2%, #ff9a55cc 53%, #ff9a5566 87%);
box-shadow: 0 10px 25px rgba(255, 127, 36, 0);
transition:
color var(--dur-btn) var(--ease),
box-shadow var(--dur-btn) var(--ease),
transform 0.5s var(--ease-out);
}

/_ White layer (opacity diye fade) _/
.specialContent .cardSection .card button::before {
content: "";
position: absolute;
inset: 0;
z-index: -1;
border-radius: inherit;
background: #ffffff;
opacity: 0;
transition: opacity var(--dur-btn) var(--ease);
}

/_ ================= HOVER STATE ================= _/
@media (hover: hover) {
.specialContent .cardSection .card:hover,
.specialContent .cardSection .card:focus-within {
z-index: 10;
transform: scale(1.2) translateZ(0);
border-radius: 44px;
box-shadow:
0 30px 60px -20px rgba(253, 134, 49, 0.55),
0 20px 40px rgba(0, 0, 0, 0.12);
}

.specialContent .cardSection .card:hover::before,
.specialContent .cardSection .card:focus-within::before {
opacity: 1;
}

/_ Shob text WHITE (button bade) _/
.specialContent .cardSection .card:hover _:not(button),
.specialContent .cardSection .card:hover _:not(button)::before,
.specialContent .cardSection .card:hover _:not(button)::after,
.specialContent .cardSection .card:focus-within _:not(button),
.specialContent .cardSection .card:focus-within _:not(button)::before,
.specialContent .cardSection .card:focus-within _:not(button)::after {
color: #ffffff !important;
}

/_ Button: white bg + orange text _/
.specialContent .cardSection .card:hover button,
.specialContent .cardSection .card:focus-within button {
color: #fd8631;
box-shadow: 0 12px 28px rgba(0, 0, 0, 0.15);
}

.specialContent .cardSection .card:hover button::before,
.specialContent .cardSection .card:focus-within button::before {
opacity: 1;
}

/_ Button er upor mouse gele halka lift _/
.specialContent .cardSection .card:hover button:hover {
transform: translateY(-2px);
box-shadow: 0 16px 32px rgba(0, 0, 0, 0.2);
}
}

/_ Touch device tap _/
.specialContent .cardSection .card:active {
transform: scale(1.12) translateZ(0);
}

/_ ================= RESPONSIVE ================= _/
@media (max-width: 1199px) {
.specialContent .cardSection .card {
padding: 56px 44px 70px;
}
.specialContent .cardSection .card:hover,
.specialContent .cardSection .card:focus-within {
transform: scale(1.12) translateZ(0);
}
}

@media (max-width: 991px) {
.specialContent .cardSection {
flex-direction: column;
gap: 32px;
}
.specialContent .cardSection .card:hover,
.specialContent .cardSection .card:focus-within {
transform: scale(1.06) translateZ(0);
}
}

/_ ================= REDUCED MOTION ================= _/
@media (prefers-reduced-motion: reduce) {
.specialContent .cardSection .card,
.specialContent .cardSection .card::before,
.specialContent .cardSection .card h1,
.specialContent .cardSection .card h2,
.specialContent .cardSection .card .para p,
.specialContent .cardSection .card button,
.specialContent .cardSection .card button::before {
transition-duration: 0.01ms !important;
}
}
