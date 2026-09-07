<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>MindBloom 🌱</title>

<style>
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    background: #f6faf6;
    color: #24352a;
    line-height: 1.6;
}

header {
    background: linear-gradient(135deg, #dcefdc, #edf7ed);
    text-align: center;
    padding: 45px 20px;
}

header h1 {
    font-size: 45px;
    margin-bottom: 8px;
}

header p {
    font-size: 18px;
}

nav {
    position: sticky;
    top: 0;
    z-index: 10;
    background: white;
    padding: 14px;
    text-align: center;
    box-shadow: 0 2px 10px rgba(0,0,0,0.08);
}

nav a {
    color: #24352a;
    text-decoration: none;
    font-weight: bold;
    margin: 0 8px;
}

nav a:hover {
    text-decoration: underline;
}

.container {
    max-width: 1100px;
    margin: auto;
    padding: 30px 18px;
}

.hero {
    text-align: center;
    padding: 30px 10px;
}

.hero h2 {
    font-size: 30px;
    margin-bottom: 10px;
}

.search {
    width: 100%;
    max-width: 600px;
    display: block;
    margin: 20px auto;
    padding: 15px;
    border: 1px solid #ccd8cc;
    border-radius: 12px;
    font-size: 16px;
}

.section-title {
    text-align: center;
    margin: 35px 0 20px;
    font-size: 28px;
}

.subject-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
    gap: 18px;
}

.card {
    background: white;
    padding: 25px;
    border-radius: 18px;
    text-decoration: none;
    color: #24352a;
    box-shadow: 0 4px 14px rgba(0,0,0,0.07);
    transition: 0.2s;
}

.card:hover {
    transform: translateY(-4px);
}

.card h3 {
    margin-bottom: 7px;
    font-size: 21px;
}

.notes-section {
    background: white;
    margin-top: 35px;
    padding: 28px;
    border-radius: 20px;
    box-shadow: 0 4px 14px rgba(0,0,0,0.06);
}

.notes-section h2 {
    margin-bottom: 18px;
    font-size: 28px;
}

.notes-section h3 {
    margin-top: 22px;
    margin-bottom: 8px;
}

.notes-section ul {
    padding-left: 25px;
}

.notes-section li {
    margin-bottom: 7px;
}

.tip {
    background: #eef7ee;
    padding: 15px;
    border-radius: 12px;
    margin-top: 15px;
}

.button {
    display: inline-block;
    margin-top: 15px;
    padding: 12px 20px;
    background: #527a5b;
    color: white;
    text-decoration: none;
    border-radius: 10px;
    font-weight: bold;
}

.button:hover {
    opacity: 0.85;
}

.checklist label {
    display: block;
    margin: 10px 0;
}

footer {
    text-align: center;
    background: #dcefdc;
    padding: 30px;
    margin-top: 40px;
}

.small {
    font-size: 14px;
    opacity: 0.8;
}

@media (max-width: 600px) {
    header h1 {
        font-size: 35px;
    }

    nav a {
        display: inline-block;
        margin: 4px;
    }

    .notes-section {
        padding: 20px;
    }
}
</style>
</head>

<body>

<header id="home">
    <h1>🌱 MindBloom</h1>
    <p>Learn • Revise • Grow</p>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#notes">Notes</a>
    <a href="#planner">Planner</a>
    <a href="#tips">Study Tips</a>
    <a href="#voice">Student Voice</a>
</nav>

<div class="container">

<section class="hero">
    <h2>Welcome to MindBloom 📚</h2>
    <p>Your simple study space for learning, revision and exam preparation.</p>

    <input
        type="text"
        id="searchBox"
        class="search"
        placeholder="🔎 Search notes..."
        onkeyup="searchNotes()"
    >
</section>

<!-- SUBJECTS -->

<h2 class="section-title" id="notes">📚 Subjects</h2>

<div class="subject-grid">

<a class="card" href="#maths">
    <h3>📐 Mathematics</h3>
    <p>IGCSE Maths revision notes</p>
</a>

<a class="card" href="#business">
    <h3>💼 Business Studies</h3>
    <p>IGCSE Business notes</p>
</a>

<a class="card" href="#economics">
    <h3>📈 Economics</h3>
    <p>IGCSE Economics notes</p>
</a>

<a class="card" href="#accounting">
    <h3>🧮 Accounting</h3>
    <p>Accounting revision</p>
</a>

<a class="card" href="#english">
    <h3>📝 English</h3>
    <p>Writing and language skills</p>
</a>

<a class="card" href="#cs">
    <h3>💻 Computer Science</h3>
    <p>IGCSE CS notes</p>
</a>

<a class="card" href="#islam">
    <h3>☪️ Islam</h3>
    <p>Revision notes</p>
</a>

<a class="card" href="#dhivehi">
    <h3>🇲🇻 Dhivehi</h3>
    <p>Language revision</p>
</a>

</div>


<!-- MATHS -->

<section class="notes-section searchable" id="maths">

<h2>📐 Mathematics</h2>

<h3>🔢 Number</h3>
<ul>
<li>Fractions</li>
<li>Decimals</li>
<li>Percentages</li>
<li>Ratio and proportion</li>
<li>Standard form</li>
<li>Indices</li>
<li>Surds</li>
<li>Bounds</li>
</ul>

<h3>📊 Algebra</h3>
<ul>
<li>Collecting like terms</li>
<li>Expanding brackets</li>
<li>Factorising</li>
<li>Linear equations</li>
<li>Simultaneous equations</li>
<li>Quadratic equations</li>
<li>Algebraic fractions</li>
<li>Sequences</li>
<li>Functions</li>
</ul>

<h3>📏 Geometry</h3>
<ul>
<li>Angles</li>
<li>Triangles</li>
<li>Quadrilaterals</li>
<li>Circle theorems</li>
<li>Similarity</li>
<li>Congruence</li>
<li>Bearings</li>
</ul>

<h3>📐 Mensuration</h3>
<ul>
<li>Perimeter</li>
<li>Area</li>
<li>Volume</li>
<li>Surface area</li>
<li>Arc length</li>
<li>Sector area</li>
</ul>

<h3>📈 Graphs</h3>
<ul>
<li>Linear graphs</li>
<li>Gradient</li>
<li>Equation of a line</li>
<li>Quadratic graphs</li>
<li>Distance-time graphs</li>
<li>Speed-time graphs</li>
</ul>

<h3>📊 Statistics & Probability</h3>
<ul>
<li>Mean</li>
<li>Median</li>
<li>Mode</li>
<li>Range</li>
<li>Probability</li>
<li>Histograms</li>
<li>Cumulative frequency</li>
</ul>

<div class="tip">
<strong>⭐ Exam tip:</strong> Show your working. Even if your final answer is wrong, working can help you earn marks.
</div>

</section>


<!-- BUSINESS -->

<section class="notes-section searchable" id="business">

<h2>💼 Business Studies</h2>

<h3>🚀 Business Activity</h3>
<ul>
<li>Purpose of business</li>
<li>Entrepreneurs</li>
<li>Business objectives</li>
<li>Stakeholders</li>
<li>Adding value</li>
</ul>

<h3>👥 People in Business</h3>
<ul>
<li>Motivation</li>
<li>Recruitment</li>
<li>Selection</li>
<li>Training</li>
<li>Leadership</li>
<li>Organisational structures</li>
</ul>

<h3>📣 Marketing</h3>
<ul>
<li>Market research</li>
<li>Market segmentation</li>
<li>Marketing mix</li>
<li>Product</li>
<li>Price</li>
<li>Promotion</li>
<li>Place</li>
</ul>

<h3>💰 Business Finance</h3>
<ul>
<li>Sources of finance</li>
<li>Revenue</li>
<li>Costs</li>
<li>Profit</li>
<li>Cash flow</li>
<li>Break-even</li>
</ul>

<h3>🌍 External Influences</h3>
<ul>
<li>Government</li>
<li>Interest rates</li>
<li>Exchange rates</li>
<li>Economic conditions</li>
<li>Technology</li>
</ul>

</section>


<!-- ECONOMICS -->

<section class="notes-section searchable" id="economics">

<h2>📈 Economics</h2>

<h3>🌱 Basic Economic Problem</h3>
<ul>
<li>Scarcity</li>
<li>Choice</li>
<li>Opportunity cost</li>
<li>Factors of production</li>
<li>Production possibility curve</li>
</ul>

<h3>🏭 Resource Allocation</h3>
<ul>
<li>Demand</li>
<li>Supply</li>
<li>Equilibrium price</li>
<li>Price mechanism</li>
<li>Elasticity</li>
</ul>

<h3>💵 Government & Economy</h3>
<ul>
<li>Economic growth</li>
<li>Inflation</li>
<li>Unemployment</li>
<li>Fiscal policy</li>
<li>Monetary policy</li>
</ul>

<h3>🌍 International Trade</h3>
<ul>
<li>Imports</li>
<li>Exports</li>
<li>Balance of payments</li>
<li>Exchange rates</li>
<li>Trade restrictions</li>
<li>Quotas</li>
<li>Embargoes</li>
</ul>

<h3>📊 Living Standards</h3>
<ul>
<li>GDP</li>
<li>GDP per capita</li>
<li>HDI</li>
<li>Poverty</li>
<li>Income distribution</li>
</ul>

</section>


<!-- ACCOUNTING -->

<section class="notes-section searchable" id="accounting">

<h2>🧮 Accounting</h2>

<h3>📚 Accounting Basics</h3>
<ul>
<li>Assets</li>
<li>Liabilities</li>
<li>Capital</li>
<li>Revenue</li>
<li>Expenses</li>
<li>Drawings</li>
</ul>

<h3>📖 Double Entry</h3>
<ul>
<li>Debit entries</li>
<li>Credit entries</li>
<li>Ledger accounts</li>
<li>Trial balance</li>
</ul>

<h3>💰 Financial Statements</h3>
<ul>
<li>Income statement</li>
<li>Statement of financial position</li>
<li>Gross profit</li>
<li>Net profit</li>
</ul>

<h3>📊 Ratios</h3>
<ul>
<li>Profitability ratios</li>
<li>Liquidity ratios</li>
<li>Efficiency ratios</li>
</ul>

</section>


<!-- ENGLISH -->

<section class="notes-section searchable" id="english">

<h2>📝 English</h2>

<h3>✍️ Writing</h3>
<ul>
<li>Articles</li>
<li>Reports</li>
<li>Reviews</li>
<li>Emails</li>
<li>Letters</li>
<li>Essays</li>
</ul>

<h3>📖 Reading</h3>
<ul>
<li>Skimming</li>
<li>Scanning</li>
<li>Finding key information</li>
<li>Understanding meaning from context</li>
</ul>

<h3>⭐ Writing Tips</h3>
<ul>
<li>Plan before writing</li>
<li>Use clear paragraphs</li>
<li>Develop your ideas</li>
<li>Use linking words</li>
<li>Check grammar</li>
<li>Check spelling</li>
</ul>

</section>


<!-- COMPUTER SCIENCE -->

<section class="notes-section searchable" id="cs">

<h2>💻 Computer Science</h2>

<h3>🖥️ Computer Systems</h3>
<ul>
<li>CPU</li>
<li>RAM</li>
<li>ROM</li>
<li>Storage</li>
<li>Input devices</li>
<li>Output devices</li>
</ul>

<h3>🔢 Data Representation</h3>
<ul>
<li>Binary</li>
<li>Denary</li>
<li>Hexadecimal</li>
<li>Character encoding</li>
<li>Images</li>
<li>Sound</li>
</ul>

<h3>🌐 Networks</h3>
<ul>
<li>LAN</li>
<li>WAN</li>
<li>Network hardware</li>
<li>Internet</li>
<li>Network security</li>
</ul>

<h3>💻 Programming</h3>
<ul>
<li>Variables</li>
<li>Data types</li>
<li>Selection</li>
<li>Iteration</li>
<li>Arrays</li>
<li>Procedures</li>
<li>Functions</li>
<li>Algorithms</li>
</ul>

</section>


<!-- ISLAM -->

<section class="notes-section searchable" id="islam">

<h2>☪️ Islam</h2>

<h3>📖 Quran</h3>
<ul>
<li>Important verses</li>
<li>Meanings</li>
<li>Lessons</li>
<li>Applications in daily life</li>
</ul>

<h3>🕌 Beliefs & Practices</h3>
<ul>
<li>Five Pillars</li>
<li>Articles of faith</li>
<li>Prayer</li>
<li>Fasting</li>
<li>Zakat</li>
<li>Hajj</li>
</ul>

<h3>⭐ Revision Method</h3>
<ul>
<li>Read the topic</li>
<li>Close the notes</li>
<li>Recall the main points</li>
<li>Check your answers</li>
</ul>

</section>


<!-- DHIVEHI -->

<section class="notes-section searchable" id="dhivehi">

<h2>🇲🇻 Dhivehi</h2>

<h3>📖 Language</h3>
<ul>
<li>Grammar</li>
<li>Vocabulary</li>
<li>Reading comprehension</li>
<li>Writing</li>
<li>Literature</li>
</ul>

<h3>✍️ Writing</h3>
<ul>
<li>Plan your ideas</li>
<li>Use paragraphs</li>
<li>Use appropriate vocabulary</li>
<li>Proofread your work</li>
</ul>

</section>


<!-- STUDY PLANNER -->

<section class="notes-section" id="planner">

<h2>📅 Study Planner</h2>

<p>Use this simple checklist when studying:</p>

<div class="checklist">

<label>
<input type="checkbox">
 Choose today's subject
</label>

<label>
<input type="checkbox">
 Review notes
</label>

<label>
<input type="checkbox">
 Use active recall
</label>

<label>
<input type="checkbox">
 Practise questions
</label>

<label>
<input type="checkbox">
 Check mistakes
</label>

<label>
<input type="checkbox">
 Review difficult topics
</label>

</div>

</section>


<!-- REVISION -->

<section class="notes-section">

<h2>✅ Revision Checklist</h2>

<ul>
<li>☐ I understand the topic</li>
<li>☐ I can explain it without notes</li>
<li>☐ I know the important formulas</li>
<li>☐ I completed practice questions</li>
<li>☐ I corrected my mistakes</li>
<li>☐ I can answer exam-style questions</li>
</ul>

</section>


<!-- STUDY TECHNIQUES -->

<section class="notes-section" id="tips">

<h2>🧠 Study Techniques</h2>

<h3>🔁 Active Recall</h3>
<p>Close your notes and try to remember the information yourself.</p>

<h3>🃏 Flashcards</h3>
<p>Put a question on one side and the answer on the other.</p>

<h3>⏱️ Pomodoro</h3>
<p>Study for a focused period, take a short break, then repeat.</p>

<h3>📚 Past Papers</h3>
<p>Practise exam questions and review your mistakes carefully.</p>

<h3>🌱 Spaced Revision</h3>
<p>Review topics repeatedly over several days instead of learning everything at once.</p>

</section>


<!-- PAST PAPERS -->

<section class="notes-section">

<h2>📝 Past Papers</h2>

<p>
Use official examination-board resources for past papers and mark schemes.
</p>

<div class="tip">
<strong>⭐ Tip:</strong> Try the paper without notes first. Then mark it and record the questions you got wrong.
</div>

</section>


<!-- STUDENT VOICE -->

<section class="notes-section" id="voice">

<h2>💬 Student Voice</h2>

<p>
Have an idea for MindBloom? Tell us what notes, features or subjects you want.
</p>

<a
    class="button"
    href="YOUR_GOOGLE_FORM_LINK_HERE"
    target="_blank"
>
    💬 Give Feedback
</a>

<p class="small">
Your feedback helps improve MindBloom for students.
</p>

</section>

</div>


<footer>
<p>🌱 MindBloom</p>
<p>Learn • Revise • Grow</p>
</footer>


<script>

function searchNotes() {

    let input = document
        .getElementById("searchBox")
        .value
        .toLowerCase();

    let sections = document.querySelectorAll(".searchable");

    sections.forEach(function(section) {

        let text = section.innerText.toLowerCase();

        if (text.includes(input)) {
            section.style.display = "";
        } else {
            section.style.display = "none";
        }

    });

}

</script>

</body>
</html>
