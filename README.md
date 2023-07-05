# LaTeX Resume Template README

This LaTeX resume template provides a clean and professional layout for creating a resume. The template is designed to be easily customizable, allowing you to input your own information and tailor the resume to your specific needs.

## Table of Contents

- [Getting Started](#getting-started)
- [Customization](#customization)
  - [Personal Information](#personal-information)
  - [Education](#education)
  - [Programming Skills](#programming-skills)
  - [Experience](#experience)
  - [Projects](#projects)
  - [Achievements](#achievements)
- [Changing the Style](#changing-the-style)

## Getting Started

To use this LaTeX resume template, follow these steps:

1. Make sure you have LaTeX installed on your system.
2. Open the LaTeX file (`resume.tex`) in your preferred LaTeX editor.
3. Customize the sections and information according to your resume.
4. Compile the LaTeX file using a LaTeX compiler to generate the PDF output.

## Customization

This section explains how to customize each section of the resume template.

### Personal Information

In the "Heading" section, you can update your personal information, such as your name, phone number, LinkedIn profile, GitHub profile, email, and portfolio. To make changes, modify the following lines:

```latex
\textbf{{\LARGE Your Name}} & \textbf{Mobile:} Your Phone Number \\
\href{https://www.linkedin.com/in/your-linkedin/}{\textbf{LinkedIn:} \textcolor{blue}{linkedin.com/in/your-linkedin/}} & \textbf{GitHub:} \href{https://github.com/your-github}{\textcolor{blue}{github.com/your-github}} \\
\href{mailto:your-email@example.com}{\textbf{Email:} \textcolor{blue}{your-email@example.com}} & \textbf{Portfolio:} \href{https://your-portfolio.com}{\textcolor{blue}{your-portfolio.com}}
```

Replace "Your Name" with your actual name, "Your Phone Number" with your phone number, "your-linkedin" with your LinkedIn profile URL, "your-github" with your GitHub profile URL, "your-email@example.com" with your email address, and "your-portfolio.com" with your portfolio URL.

### Education

In the "Education" section, you can list your educational background. To add or modify education details, follow the provided example:

```latex
\resumeSubheading
{Your University/College}{Location}
{Degree - Major; CGPA: Your CGPA/GPA}{Month Year - Month Year}
```

Replace "Your University/College" with the name of your university or college, "Location" with the location of your institution, "Degree - Major" with your degree and major, and "Your CGPA/GPA" with your CGPA or GPA. Repeat this structure for each education entry you want to include.

### Programming Skills

In the "Programming Skills" section, you can showcase your programming skills. To add or modify programming skills, use the following structure:

```latex
\item{\textbf{Languages}: Your Languages}
\item{\textbf{Frameworks}: Your Frameworks}
\item{\textbf{Databases}: Your Databases}
\item{\textbf{Tools}: Your Tools}
```

Replace "Your Languages" with the programming languages you know, "Your Frameworks" with the frameworks you are familiar with, "Your Databases" with the databases you have experience in, and "Your Tools" with the tools you have used.

### Experience

In the "Experience" section, you can list

 your work experience. To add or modify experience entries, follow this structure:

```latex
\resumeSubheading
{Company/Organization}{Location}
{Position}{Month Year - Month Year}
\resumeItemListStart
  \resumeItem{Responsibility}
  {Description of your responsibilities}
\resumeItemListEnd
```

Replace "Company/Organization" with the name of the company or organization, "Location" with the location, "Position" with your position or role, and "Month Year - Month Year" with the duration of your employment. Add a description of your responsibilities using the `\resumeItem` command within the `\resumeItemListStart` and `\resumeItemListEnd` environment.

### Projects

In the "Projects" section, you can showcase your projects. To add or modify project entries, use the following structure:

```latex
\item{\textbf{Project Title}}
\resumeItemListStart
  \item Description of the project
\resumeItemListEnd
\textbf{Tech}: Technologies used for the project
\hfill \textcolor{blue}{\href{https://project-url.com}{Check it out...}}
```

Replace "Project Title" with the title of your project and provide a description using the `\item` command within the `\resumeItemListStart` and `\resumeItemListEnd` environment. Specify the technologies used in the project under the "Tech" line, and update the URL within `\href{}` to link to your project.

### Achievements

In the "Achievements" section, you can list your notable achievements. To add or modify achievements, use the following structure:

```latex
\item Achievement description
```

Replace "Achievement description" with a brief description of your achievement. Repeat this structure for each achievement you want to include.

## Changing the Style

This resume template uses predefined styles and formatting. If you wish to change the style, you can modify various aspects of the template, such as fonts, colors, margins, and section formatting.

To change fonts, you can search for the font-related commands, such as `\textbf`, `\textit`, and `\scshape`, and replace them with your preferred font commands.

To change colors, you can modify the color names defined in the `\usepackage[usenames,dvipsnames]{color}` command. The color names are used for hyperlinks and section rules.

To adjust margins, you can modify the `\addtolength` commands under the "Adjust margins" section. This allows you to change the page margins according to your preference.

To modify section formatting, you can adjust the `\titleformat` command under the "Section formatting" section. This command controls the appearance of section headings.

Remember to maintain the LaTex code structure and syntax while making changes to ensure the template functions correctly.

### Example 1: Changing Fonts

To change the font to a sans-serif font, replace the font commands in the "Heading" section with the following:

```latex
\textsf{{\LARGE Your Name}} & \textsf{Mobile:} Your Phone Number \\
\href{https://www.linkedin.com/in/your-linkedin/}{\textsf{LinkedIn:} \textcolor{blue}{linkedin.com/in/your-linkedin/}} & \textsf{GitHub:} \href{https://github.com/your-github}{\textcolor{blue}{github.com/your-github}} \\
\href{mailto:your-email@example.com}{\textsf{Email:} \textcolor{blue}{your-email@example.com}} & \textsf{Portfolio:} \href{https://your-portfolio.com}{\textcolor{blue}{your-portfolio.com}}
```

### Example 2: Changing Colors

To change

 the color of hyperlinks to red, modify the color name in the `\usepackage[usenames,dvipsnames]{color}` command to:

```latex
\usepackage[usenames,dvipsnames]{color}
\definecolor{blue}{rgb}{0,0,1}  % Replace with desired color (e.g., red)
```

### Example 3: Adjusting Margins

To increase the left margin by 0.5 inches, modify the `\addtolength` command under the "Adjust margins" section as follows:

```latex
\addtolength{\oddsidemargin}{-0.5in}
\addtolength{\evensidemargin}{-0.5in}
```

These examples provide a starting point for customizing the template to suit your preferences. Feel free to experiment and make further changes as desired.

Happy resume building!