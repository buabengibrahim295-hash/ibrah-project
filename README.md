
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CCTU Computer Science - Level 200 Directory</title>
    <style>
        :root {
            --primary-brown: #5d4037;
            --light-brown: #8d6e63;
            --bg-beige: #f5f5dc;
            --white: #ffffff;
            --shadow: 0 4px 12px rgba(0,0,0,0.08);
        }

        /* Smooth Scrolling */
        html { scroll-behavior: smooth; }

        body { 
            background-color: var(--bg-beige); 
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; 
            margin: 0; 
            padding: 0; 
            color: #3e2723; 
        }

        header { 
            max-width: 1000px; 
            margin: 40px auto 20px; 
            background: var(--white); 
            padding: 40px; 
            border-radius: 20px; 
            text-align: center; 
            box-shadow: var(--shadow); 
        }

        .logo { width: 160px; height: auto; margin-bottom: 20px; }
        h1 { font-size: 2rem; margin: 10px 0; color: var(--primary-brown); }

        .history { 
            text-align: left; 
            border-top: 2px solid #eee; 
            margin-top: 25px; 
            padding-top: 20px; 
            line-height: 1.7; 
            font-size: 0.95rem;
            color: #555;
        }

        /* Search Bar Styling */
        .search-container {
            position: sticky;
            top: 20px;
            z-index: 100;
            max-width: 600px;
            margin: 0 auto 40px;
            padding: 0 20px;
        }

        #studentSearch {
            width: 100%;
            padding: 15px 25px;
            font-size: 1rem;
            border: 2px solid var(--white);
            border-radius: 50px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.1);
            outline: none;
            transition: 0.3s;
        }

        /* Grid Layout */
        .student-container { 
            display: grid; 
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr)); 
            gap: 25px; 
            max-width: 1200px; 
            margin: 0 auto; 
            padding: 0 20px;
        }

        .student-card { 
            background: var(--white); 
            padding: 20px; 
            border-radius: 15px; 
            display: flex; 
            align-items: center; 
            gap: 20px;
            box-shadow: var(--shadow); 
            border: 1px solid rgba(215, 204, 200, 0.5);
            transition: all 0.3s ease;
        }

        .student-card:hover { 
            transform: translateY(-8px); 
            box-shadow: 0 12px 24px rgba(0,0,0,0.12);
        }

        .avatar { 
            width: 65px; height: 65px; border-radius: 50%; 
            overflow: hidden; background: #eee; border: 3px solid var(--bg-beige);
            flex-shrink: 0;
        }

        .avatar img { width: 100%; height: 100%; object-fit: cover; }
        .info { text-align: left; }
        .name { display: block; font-weight: 700; font-size: 0.95rem; text-transform: uppercase; color: var(--primary-brown); margin-bottom: 4px;}
        .index { color: var(--light-brown); font-size: 0.85rem; font-family: 'Courier New', monospace; }

        /* Review Section */
        .review-section { 
            max-width: 650px; 
            margin: 80px auto 40px; 
            background: var(--white); 
            padding: 40px; 
            border-radius: 20px; 
            box-shadow: var(--shadow); 
        }

        input[type="text"], select, textarea { 
            width: 100%; padding: 14px; margin: 12px 0; border: 1px solid #eee; 
            border-radius: 10px; box-sizing: border-box; font-size: 1rem;
        }
        
        .btn { 
            width: 100%; padding: 16px; background: var(--primary-brown); 
            color: white; border: none; border-radius: 10px; cursor: pointer; font-weight: bold; 
        }

        /* Back to Top Button Styling */
        #backToTop {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 50px;
            height: 50px;
            background: var(--primary-brown);
            color: white;
            border: none;
            border-radius: 50%;
            font-size: 24px;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            display: none; /* Hidden by default */
            z-index: 1000;
            transition: 0.3s;
        }

        #backToTop:hover { background: #3e2723; transform: scale(1.1); }

        footer { text-align: center; color: var(--light-brown); padding: 40px 20px; font-size: 0.9rem; }
        .hidden { display: none !important; }
    </style>
</head>
<body>

<div id="top"></div>

<header>
    <img src="image/cctu.jfif" width="300" height="300">
    <h1>Department of Computer Science</h1>
    <div class="history">
        <h3>Academic History</h3>
        <p>The history of Cape Coast Technical University (CCTU) is a journey of evolution from a vocational training center to a premier degree-granting institution. Established in 1984 as a Second Cycle Technical Institute, its primary mission was to bridge the gap in technical skills within Ghana’s Central Region.

<h4>Key Milestones</h4>
 In 1992 Under the PNDC Law 321, the school was upgraded to Cape Coast Polytechnic. This shift allowed the institution to offer tertiary-level programs, specifically Higher National Diplomas (HND).

2016: A landmark transformation occurred when the Technical Universities Act (Act 922) converted the polytechnic into a fully-fledged university. This enabled CCTU to award its own degrees, including Bachelor of Technology (B.Tech) and Master of Technology (M.Tech) certifications.

Academic Focus
CCTU has distinguished itself through a hands-on, competency-based training model. The university is organized into several key faculties:

Engineering (Mechanical, Civil, and Electrical)

Applied Sciences and Technology

Business and Management Studies

Built and Natural Environment

Today, the university is recognized for its niche focus on Renewable Energy and Entrepreneurship, preparing students to drive industrial growth and innovation in Ghana and beyond.</p>
    </div>
</header>

<div class="search-container">
    <input type="text" id="studentSearch" placeholder="Search by name or index number..." onkeyup="filterStudents()">
</div>

<div class="student-container" id="studentGrid">
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">AMOAKO KUMI STANLEY</span><span class="index">0224DCS0015</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">INKOOM SOLOMON</span><span class="index">0224DCS0002</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">AGGREY BOSSMAN MILORD</span><span class="index">0224DCS0012</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">NAAGMENSONG GYAMFI PAUL</span><span class="index">0224DCS0021</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">YEBOAH KWADJO BISMARK SAMUEL</span><span class="index">0224DCS0014</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">BOSU ADDISON FRANCIS</span><span class="index">0224DCS0017</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">YIRENKYI SAMUEL</span><span class="index">0224DCS0007</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">AMOAH PRINCE</span><span class="index">0224DCS0004</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">ΑΚΡΑΒΙΟ FELIX GODSWILL</span><span class="index">0224DCS0013</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">ANANI DELALI RICHMOND</span><span class="index">0224DCS0009</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">OTOO JUNIOR JOSEPΗ</span><span class="index">0224DCS0025</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">BUABENG IBRAHIM</span><span class="index">0224DCS0036</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">APPIAH AKYEN REGINAID</span><span class="index">0224DCS0026</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">ABAAMI WEMONIAMO EMMANUEL</span><span class="index">0224DCS0006</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">ALEX OBOH NYAME</span><span class="index">0224DCS0043</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">SAM ABIGAIL</span><span class="index">0224DCS0011</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">ACHEAMPONG ERNEST</span><span class="index">0224DCS0010</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">MICHAEL DARKO ANNOM</span><span class="index">0224DCS0001</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">AGYEMANG OSEI NANA</span><span class="index">0224DCS0029</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">ENOCH MENSAH</span><span class="index">0224DCS0028</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">ALEX QUANSAH</span><span class="index">0224DCS0005</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">ASARE FELIX</span><span class="index">0224DCS0024</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">PROSPER OFORI MANTEAW</span><span class="index">0224DCS0020</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">RANSFORD EGYIR</span><span class="index">0224DCS0018</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">DANIEL OSEI JUNIOR</span><span class="index">0224DCS0032</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">JOEL ABBAN</span><span class="index">0224DCS0019</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">RICHARD ARKORFUL</span><span class="index">0224DCS0033</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">COLLINS OPOKU YEBОАН</span><span class="index">0224DCS0022</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">EMMANUEL ARTHUR</span><span class="index">0224DCS0035</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">SETH TENADU</span><span class="index">0224DCS0035</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">GREGORY FIIFI SOWAH</span><span class="index">0224DCS0027</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">EMMANUEL CLINTON</span><span class="index">0224DCS0033</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">EMMANUEL BANS</span><span class="index">0224DCS0034</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">ASAMOAH AMPONSAH GERTRUDE</span><span class="index">0224DCS0036</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">GODSWAY EGLI</span><span class="index">0224DCS0037</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">SOLOMON BROWN QUAYE</span><span class="index">0224DCS0023</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">IBRAHIM MOHAMMED</span><span class="index">0224DCS0042</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">EMMANUEL ATWERI OPARE</span><span class="index">0224DCS0045</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">CALEB FIANKO BEKOE</span><span class="index">0224DCS0046</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">CHRISTIAN YARTEY</span><span class="index">0224DCS0046</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">OSBORNE AMPONSAH VAN</span><span class="index">0224DCS0047</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">RUTH NYARKO BOAKYE</span><span class="index">0224DCS0040</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">OLIVER AMOAH KOBBIE</span><span class="index">0224DCS0048</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">MICHAEL MENSAH</span><span class="index">0224DCS0050</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">EMMANUELLA MORGAN</span><span class="index">0224DCS0003</span></div></div>
    <div class="student-card"><div class="avatar"><img src="image/c.jfif"></div><div class="info"><span class="name">SETH AFFRISAH</span><span class="index">0224DCS0039</span></div></div>
</div>

<div class="review-section">
    <h2>Review & Feedback</h2>
    <input type="text" placeholder="Full Name">
    <select title="Rating Options">
        <option>Rating: 5 Stars</option>
        <option>Rating: 4 Stars</option>
        <option>Rating: 3 Stars</option>
    </select>
    <textarea placeholder="Write your review here..."></textarea>
    <button class="btn" onclick="alert('Posted Successfully!')">Post Review</button>
</div>

<button id="backToTop" onclick="scrollToTop()" title="Go to top">↑</button>

<footer>
    &copy; 2026 Cape Coast Technical University | Computer Science Dept.
</footer>

<script>
    // Search Functionality
    function filterStudents() {
        let input = document.getElementById('studentSearch').value.toLowerCase();
        let cards = document.getElementsByClassName('student-card');
        
        for (let i = 0; i
