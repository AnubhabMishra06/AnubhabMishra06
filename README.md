<svg width="1600" height="500" viewBox="0 0 1600 500" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
  <defs>
    <linearGradient id="spaceBg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#020308"/>
      <stop offset="50%" stop-color="#060a1a"/>
      <stop offset="100%" stop-color="#0a1228"/>
    </linearGradient>
    <radialGradient id="nebulaBlue" cx="75%" cy="35%" r="55%">
      <stop offset="0%" stop-color="#0A84FF" stop-opacity="0.22"/>
      <stop offset="60%" stop-color="#0A84FF" stop-opacity="0.05"/>
      <stop offset="100%" stop-color="#0A84FF" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="nebulaPurple" cx="25%" cy="80%" r="50%">
      <stop offset="0%" stop-color="#7c3aed" stop-opacity="0.13"/>
      <stop offset="100%" stop-color="#7c3aed" stop-opacity="0"/>
    </radialGradient>

    <linearGradient id="textGlow" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#ffffff"/>
      <stop offset="100%" stop-color="#cfe6ff"/>
    </linearGradient>
    <linearGradient id="dividerGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#0A84FF" stop-opacity="0"/>
      <stop offset="50%" stop-color="#37b6ff" stop-opacity="1"/>
      <stop offset="100%" stop-color="#0A84FF" stop-opacity="0"/>
    </linearGradient>
    <radialGradient id="orbGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#37b6ff" stop-opacity="0.35"/>
      <stop offset="60%" stop-color="#0A84FF" stop-opacity="0.1"/>
      <stop offset="100%" stop-color="#0A84FF" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="coreGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#ffffff"/>
      <stop offset="40%" stop-color="#9fe0ff"/>
      <stop offset="100%" stop-color="#0A84FF" stop-opacity="0"/>
    </radialGradient>

    <filter id="blurSoft" x="-50%" y="-50%" width="200%" height="200%"><feGaussianBlur stdDeviation="5"/></filter>
    <filter id="blurStrong" x="-50%" y="-50%" width="200%" height="200%"><feGaussianBlur stdDeviation="20"/></filter>
    <filter id="textGlowFilter" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="3.4" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="panelShadow" x="-50%" y="-50%" width="200%" height="200%">
      <feDropShadow dx="0" dy="4" stdDeviation="6" flood-color="#000000" flood-opacity="0.45"/>
    </filter>

    <clipPath id="frame"><rect width="1600" height="500"/></clipPath>
    <clipPath id="ringClip"><circle cx="0" cy="0" r="150"/></clipPath>
  </defs>

  <g clip-path="url(#frame)">
    <rect width="1600" height="500" fill="url(#spaceBg)"/>
    <rect width="1600" height="500" fill="url(#nebulaBlue)"/>
    <rect width="1600" height="500" fill="url(#nebulaPurple)"/>

    <!-- starfield twinkle -->
    <g fill="#ffffff">
      <circle cx="80" cy="40" r="1.1" opacity="0.7"><animate attributeName="opacity" values="0.2;0.9;0.2" dur="3s" repeatCount="indefinite"/></circle>
      <circle cx="260" cy="90" r="1" opacity="0.6"><animate attributeName="opacity" values="0.8;0.2;0.8" dur="4s" repeatCount="indefinite"/></circle>
      <circle cx="430" cy="30" r="1.3" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="2.6s" repeatCount="indefinite"/></circle>
      <circle cx="610" cy="120" r="1" opacity="0.5"><animate attributeName="opacity" values="0.6;0.1;0.6" dur="3.4s" repeatCount="indefinite"/></circle>
      <circle cx="120" cy="200" r="1.2" opacity="0.7"><animate attributeName="opacity" values="0.2;0.8;0.2" dur="3.8s" repeatCount="indefinite"/></circle>
      <circle cx="40" cy="340" r="1" opacity="0.6"><animate attributeName="opacity" values="0.9;0.3;0.9" dur="2.9s" repeatCount="indefinite"/></circle>
      <circle cx="220" cy="420" r="1.3" opacity="0.7"><animate attributeName="opacity" values="0.3;0.9;0.3" dur="3.1s" repeatCount="indefinite"/></circle>
      <circle cx="700" cy="60" r="1.1" opacity="0.6"><animate attributeName="opacity" values="0.2;0.9;0.2" dur="3.3s" repeatCount="indefinite"/></circle>
      <circle cx="1500" cy="430" r="1.1" opacity="0.6"><animate attributeName="opacity" values="0.2;0.9;0.2" dur="3.7s" repeatCount="indefinite"/></circle>
      <circle cx="1550" cy="70" r="1.2" opacity="0.7"><animate attributeName="opacity" values="0.3;0.9;0.3" dur="2.8s" repeatCount="indefinite"/></circle>
    </g>

    <!-- parallax streak lines -->
    <g stroke="#9fc8ff" stroke-width="1" opacity="0.28">
      <line x1="-50" y1="100" x2="-10" y2="100">
        <animate attributeName="x1" values="-50;1650" dur="9s" repeatCount="indefinite"/>
        <animate attributeName="x2" values="-10;1690" dur="9s" repeatCount="indefinite"/>
      </line>
      <line x1="-80" y1="440" x2="-30" y2="440">
        <animate attributeName="x1" values="-80;1620" dur="12s" repeatCount="indefinite" begin="4s"/>
        <animate attributeName="x2" values="-30;1670" dur="12s" repeatCount="indefinite" begin="4s"/>
      </line>
    </g>

    <!-- ================= LEFT: NAME (large, animated) ================= -->
    <g filter="url(#textGlowFilter)">
      <text x="75" y="225" font-family="Helvetica, Arial, sans-serif" font-weight="800" font-size="92" letter-spacing="1" fill="url(#textGlow)" opacity="0">
        ANUBHAB
        <animate attributeName="opacity" values="0;0;1;1" keyTimes="0;0.04;0.26;1" dur="3s" begin="0s" fill="freeze"/>
        <animateTransform attributeName="transform" type="translate" values="-50,0;-50,0;0,0" keyTimes="0;0.04;0.26" dur="3s" begin="0s" fill="freeze" additive="sum"/>
      </text>
      <text x="75" y="310" font-family="Helvetica, Arial, sans-serif" font-weight="800" font-size="92" letter-spacing="1" fill="url(#textGlow)" opacity="0">
        MISHRA
        <animate attributeName="opacity" values="0;0;1;1" keyTimes="0;0.16;0.4;1" dur="3s" begin="0s" fill="freeze"/>
        <animateTransform attributeName="transform" type="translate" values="-50,0;-50,0;0,0" keyTimes="0;0.16;0.4" dur="3s" begin="0s" fill="freeze" additive="sum"/>
      </text>
      <animate attributeName="opacity" values="1;0.82;1" dur="4s" begin="3.2s" repeatCount="indefinite"/>
    </g>

    <rect x="75" y="320" width="0" height="3" fill="#37b6ff" opacity="0.85">
      <animate attributeName="width" values="0;560;560" keyTimes="0;0.5;1" dur="1.2s" begin="0.2s" fill="freeze"/>
      <animate attributeName="opacity" values="0.85;0.2" dur="1.4s" begin="1.4s" fill="freeze"/>
    </rect>

    <text x="78" y="360" font-family="Helvetica, Arial, sans-serif" font-size="20" fill="#a9c6ec" letter-spacing="1" opacity="0">
      Information Technology Student
      <animate attributeName="opacity" values="0;0;1" keyTimes="0;0.69;1" dur="2.4s" begin="1.6s" fill="freeze"/>
    </text>

    <rect x="78" y="382" width="430" height="1.6" fill="url(#dividerGrad)">
      <animate attributeName="width" values="0;430" dur="1s" begin="2.1s" fill="freeze"/>
    </rect>
    <circle cx="78" cy="383" r="2.6" fill="#37b6ff">
      <animate attributeName="opacity" values="1;0.3;1" dur="2.4s" repeatCount="indefinite"/>
    </circle>

    <text x="78" y="412" font-family="Helvetica, Arial, sans-serif" font-weight="300" font-size="16" fill="#6f93c2" letter-spacing="0.5" opacity="0">
      Java &#8226; DSA &#8226; Software Engineering &#8226; AI &amp; Machine Learning
      <animate attributeName="opacity" values="0;0;1" keyTimes="0;0.5;1" dur="1.6s" begin="2.6s" fill="freeze"/>
    </text>

    <text x="78" y="442" font-family="Menlo, monospace" font-size="11" fill="#3f6fb0" opacity="0">
      STATUS: ONLINE <tspan fill="#37b6ff">// BUILDING</tspan>
      <animate attributeName="opacity" values="0;0;0.7" keyTimes="0;0.6;1" dur="1.4s" begin="3s" fill="freeze"/>
    </text>
    <rect x="241" y="430" width="8" height="14" fill="#37b6ff" opacity="0">
      <animate attributeName="opacity" values="0;0;0.9;0.9;0;0" keyTimes="0;0.4;0.41;0.7;0.71;1" dur="1.1s" begin="3.4s" repeatCount="indefinite"/>
    </rect>

    <!-- ================= RIGHT: ROTATING DEV ORBIT SYSTEM ================= -->
    <g transform="translate(1190,250)">
      <circle r="240" fill="url(#orbGlow)" filter="url(#blurStrong)"/>
      <ellipse rx="230" ry="230" fill="none" stroke="#1f3a5f" stroke-width="1" opacity="0.4"/>
      <ellipse rx="170" ry="170" fill="none" stroke="#1f3a5f" stroke-width="1" opacity="0.3"/>

      <g>
        <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="26s" repeatCount="indefinite"/>
        <ellipse rx="210" ry="80" fill="none" stroke="#37b6ff" stroke-width="1.3" opacity="0.55"/>
        <g transform="translate(210,0)">
          <circle r="20" fill="#0d1929" stroke="#37b6ff" stroke-width="1.4" filter="url(#panelShadow)"/>
          <text x="0" y="5" font-family="Helvetica,Arial,sans-serif" font-weight="700" font-size="13" fill="#9fe0ff" text-anchor="middle">Jv</text>
        </g>
        <g transform="translate(-210,0)">
          <circle r="20" fill="#0d1929" stroke="#37b6ff" stroke-width="1.4" filter="url(#panelShadow)"/>
          <text x="0" y="5" font-family="Helvetica,Arial,sans-serif" font-weight="700" font-size="12" fill="#9fe0ff" text-anchor="middle">Py</text>
        </g>
      </g>

      <g>
        <animateTransform attributeName="transform" type="rotate" from="360" to="0" dur="20s" repeatCount="indefinite"/>
        <ellipse rx="150" ry="150" fill="none" stroke="#37b6ff" stroke-width="1" opacity="0.4"/>
        <g transform="translate(0,-150)">
          <circle r="17" fill="#0d1929" stroke="#37b6ff" stroke-width="1.2" filter="url(#panelShadow)"/>
          <text x="0" y="4.5" font-family="Helvetica,Arial,sans-serif" font-weight="700" font-size="10" fill="#9fe0ff" text-anchor="middle">Git</text>
        </g>
        <g transform="translate(0,150)">
          <circle r="17" fill="#0d1929" stroke="#37b6ff" stroke-width="1.2" filter="url(#panelShadow)"/>
          <text x="0" y="4.5" font-family="Helvetica,Arial,sans-serif" font-weight="700" font-size="9" fill="#9fe0ff" text-anchor="middle">SQL</text>
        </g>
        <g transform="translate(106,106)">
          <circle r="16" fill="#0d1929" stroke="#37b6ff" stroke-width="1.2" filter="url(#panelShadow)"/>
          <text x="0" y="4.2" font-family="Helvetica,Arial,sans-serif" font-weight="700" font-size="9" fill="#9fe0ff" text-anchor="middle">AI</text>
        </g>
        <g transform="translate(-106,-106)">
          <circle r="16" fill="#0d1929" stroke="#37b6ff" stroke-width="1.2" filter="url(#panelShadow)"/>
          <text x="0" y="4.2" font-family="Helvetica,Arial,sans-serif" font-weight="700" font-size="8" fill="#9fe0ff" text-anchor="middle">ML</text>
        </g>
      </g>

      <g>
        <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="13s" repeatCount="indefinite"/>
        <ellipse rx="95" ry="95" fill="none" stroke="#37b6ff" stroke-width="0.8" opacity="0.35"/>
        <circle cx="95" cy="0" r="4" fill="#9fe0ff"/>
        <circle cx="-95" cy="0" r="3" fill="#37b6ff" opacity="0.8"/>
      </g>

      <g>
        <circle r="58" fill="url(#coreGlow)" opacity="0.5">
          <animate attributeName="opacity" values="0.35;0.6;0.35" dur="4s" repeatCount="indefinite"/>
        </circle>
        <g stroke="#bfe3ff" stroke-width="1" fill="none" opacity="0.8">
          <ellipse rx="52" ry="52"/>
          <ellipse rx="52" ry="18"/>
          <ellipse rx="52" ry="34">
            <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="9s" repeatCount="indefinite"/>
          </ellipse>
          <ellipse rx="18" ry="52"/>
          <ellipse rx="34" ry="52">
            <animateTransform attributeName="transform" type="rotate" from="0" to="-360" dur="11s" repeatCount="indefinite"/>
          </ellipse>
        </g>
        <g fill="#0A84FF">
          <circle cx="0" cy="0" r="6">
            <animate attributeName="opacity" values="0.6;1;0.6" dur="2.4s" repeatCount="indefinite"/>
          </circle>
          <circle cx="22" cy="-14" r="2.6"><animate attributeName="opacity" values="0.3;1;0.3" dur="3s" repeatCount="indefinite"/></circle>
          <circle cx="-24" cy="10" r="2.6"><animate attributeName="opacity" values="1;0.3;1" dur="2.6s" repeatCount="indefinite"/></circle>
          <circle cx="6" cy="26" r="2.2"><animate attributeName="opacity" values="0.4;1;0.4" dur="3.4s" repeatCount="indefinite"/></circle>
        </g>
      </g>

      <g stroke="#37b6ff" stroke-width="0.8" opacity="0.25">
        <line x1="0" y1="0" x2="160" y2="-40">
          <animate attributeName="opacity" values="0.1;0.4;0.1" dur="3.6s" repeatCount="indefinite"/>
        </line>
        <line x1="0" y1="0" x2="-150" y2="60">
          <animate attributeName="opacity" values="0.4;0.1;0.4" dur="4.2s" repeatCount="indefinite"/>
        </line>
      </g>

      <g fill="#9fc8ff">
        <circle cx="-260" cy="-120" r="1.5" opacity="0.6"><animate attributeName="cy" values="-120;-140;-120" dur="8s" repeatCount="indefinite"/></circle>
        <circle cx="270" cy="140" r="1.4" opacity="0.55"><animate attributeName="cy" values="140;160;140" dur="9s" repeatCount="indefinite"/></circle>
        <circle cx="-230" cy="160" r="1.3" opacity="0.5"><animate attributeName="cy" values="160;180;160" dur="10s" repeatCount="indefinite"/></circle>
        <circle cx="250" cy="-160" r="1.4" opacity="0.55"><animate attributeName="cy" values="-160;-180;-160" dur="8.5s" repeatCount="indefinite"/></circle>
      </g>
    </g>

    <rect x="-400" y="0" width="180" height="500" fill="#ffffff" opacity="0.025" filter="url(#blurSoft)">
      <animateTransform attributeName="transform" type="translate" values="0,0;2200,0" dur="10s" begin="1.5s" repeatCount="indefinite"/>
    </rect>

    <rect width="1600" height="500" fill="#000000" opacity="0.14" style="mix-blend-mode:multiply"/>
  </g>
</svg>

<br/>

## About Me

I'm an Information Technology student at **Haldia Institute of Technology**, graduating in 2028, with a strong current focus on **Java** and a steady, daily practice of **Data Structures & Algorithms**.

I'm drawn to **Software Engineering** as a discipline, and to **product thinking** as a way of asking why something is worth building, not just how. My long-term goal is to move into **Artificial Intelligence & Machine Learning**, but I believe in mastering fundamentals before specializing — so that's where my time goes right now.

This profile is where I'm learning publicly: tracking real progress, not polishing an image. I'm not claiming expertise here, just consistency.

<br/>

## Current Focus

<table>
<tr>
<td valign="top" width="50%">

**Currently Building**
- Java
- Object-Oriented Programming
- Data Structures & Algorithms
- Git & GitHub

</td>
<td valign="top" width="50%">

**Currently Exploring**
- Web Development
- Software Engineering
- Open Source
- Problem Solving

</td>
</tr>
</table>

<br/>

## Tech Stack

**Programming Languages**

<img src="https://skillicons.dev/icons?i=java,python,c" />

**Frontend**

<img src="https://skillicons.dev/icons?i=html,css,javascript" />

**Developer Tools**

<img src="https://skillicons.dev/icons?i=git,github,vscode,idea" />

**Currently Exploring**

<img src="https://skillicons.dev/icons?i=mysql" />

<br/>

## AI Tools

I use AI tools as part of my regular learning and workflow — for research, coding assistance, documentation, and brainstorming.

<p>
<img src="https://img.shields.io/badge/ChatGPT-111111?style=for-the-badge&logo=openai&logoColor=white" />
<img src="https://img.shields.io/badge/Claude-111111?style=for-the-badge&logo=anthropic&logoColor=white" />
<img src="https://img.shields.io/badge/Gemini-111111?style=for-the-badge&logo=googlegemini&logoColor=8E75FF" />
<img src="https://img.shields.io/badge/Perplexity-111111?style=for-the-badge&logo=perplexity&logoColor=20808D" />
<img src="https://img.shields.io/badge/Grok-111111?style=for-the-badge&logo=x&logoColor=white" />
</p>
<p>
<img src="https://img.shields.io/badge/NotebookLM-111111?style=for-the-badge&logo=googlecloud&logoColor=4285F4" />
<img src="https://img.shields.io/badge/Cursor-111111?style=for-the-badge&logo=cursor&logoColor=white" />
<img src="https://img.shields.io/badge/GitHub_Copilot-111111?style=for-the-badge&logo=githubcopilot&logoColor=white" />
<img src="https://img.shields.io/badge/Gamma-111111?style=for-the-badge&logo=googlegamma&logoColor=white" />
<img src="https://img.shields.io/badge/Canva_AI-111111?style=for-the-badge&logo=canva&logoColor=00C4CC" />
<img src="https://img.shields.io/badge/ElevenLabs-111111?style=for-the-badge&logo=elevenlabs&logoColor=white" />
</p>

<br/>

## Learning Roadmap

<div align="center">

```
Java
  │
  ▼
Data Structures & Algorithms
  │
  ▼
Object-Oriented Programming
  │
  ▼
Git & GitHub
  │
  ▼
Web Development
  │
  ▼
Projects
  │
  ▼
System Design Fundamentals
  │
  ▼
Artificial Intelligence
  │
  ▼
Machine Learning
```

</div>

<br/>

## Coding Profiles

<div align="center">

[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/AjUnSTkSQd/)

Solving problems consistently as part of daily DSA practice.

</div>

<br/>

## Featured Projects

I'm currently building high-quality projects that showcase my learning journey. They will be pinned here as they are completed.

<br/>

## Product Thinking

Alongside engineering, I'm developing an interest in how good products get built, not just how they're coded:

- Product Thinking
- User-Centered Design
- Product Management Basics
- Technology Strategy
- Digital Products

<br/>


## Connect With Me

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AnubhabMishra06)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://in.linkedin.com/in/anubhab-mishra-2334a1391)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/AjUnSTkSQd/)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/itsanubhab108)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mishraanubhab18@gmail.com)

</div>

<br/>

<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:111111,100:0A84FF&height=120&section=footer&text=Thanks%20for%20visiting%20my%20profile&fontSize=16&fontColor=ffffff&fontAlignY=75" />

Always learning. Always building. Always improving.

</div>
