# Product Requirements Document (PRD): AI-Generated Agency Portfolio Website

## 1. Introduction & Overview

This document outlines the requirements for an AI-generated, high-performance agency portfolio website. The primary goal is to create a compelling digital presence that effectively showcases our expertise in MERN Stack Web Development, CMS Integration, Application Development, and Automation (Python/n8n). The website will serve as a lead generation tool, converting visitors into qualified client inquiries by demonstrating technical prowess, project success, and a professional agency image.

## 2. Target Audience

The website is designed to appeal to several key demographics. Small to Medium-sized Businesses (SMBs) seeking custom web solutions, CMS implementations, or process automation form a primary segment. Startups requiring rapid Minimum Viable Product (MVP) development using the MERN stack are another crucial target. Furthermore, entrepreneurs looking for bespoke application development or workflow automation to scale their operations will find relevant solutions. Ultimately, the content must resonate with decision-makers, such as CEOs, CTOs, and Project Managers, who prioritize clear communication, proven results, and efficient project delivery.

## 3. Key Features & Functionality

The website must include several core pages to guide the user journey effectively. The **Homepage** requires an engaging hero section, a clear value proposition, a quick overview of services, featured projects, client testimonials, and a prominent Call-to-Action (CTA). The **Services Page** will provide a detailed breakdown of each offering, outlining benefits, processes, and relevant technologies. The **Portfolio/Case Studies Page** is the most critical section for conversion, showcasing successful projects with in-depth analysis. An **About Us Page** will introduce the agency, highlighting the combined expertise of the talent agent and the lead developer, emphasizing core values and unique selling propositions. Finally, a **Contact Page** must offer an easy-to-use contact form, direct contact information, and ideally, a scheduling tool for immediate consultations.

### 3.1. Portfolio/Case Study Structure

Each case study must follow a structured format to maximize impact and clearly communicate value. The following table outlines the required components for every portfolio entry:

| Component | Description |
| :--- | :--- |
| **Project Title & Client** | A clear, concise title and the client's name (anonymized if necessary). |
| **Problem Statement** | A detailed explanation of the specific challenge or pain point the client faced. |
| **Our Solution** | A comprehensive description of how the problem was addressed using our specific services. |
| **Technologies Used** | A specific list of MERN components, CMS platforms, n8n nodes, or Python libraries utilized. |
| **Key Features** | A breakdown of the main functionalities developed and implemented. |
| **Results & Impact** | Quantifiable outcomes, such as increased efficiency, improved performance, or cost savings. |
| **Visual Evidence** | High-quality screenshots, interactive demos, Loom videos, or architectural diagrams. |

## 4. Design & User Experience (UX) Guidelines

The design must reflect a modern, high-end technology agency. The aesthetic should be clean, minimalist, and professional, utilizing a sophisticated color palette (e.g., deep blues, crisp whites, and strategic accent colors). Typography must be highly legible, favoring modern sans-serif fonts.

The user experience must be frictionless. Navigation should be intuitive, allowing users to find relevant case studies or contact information within one or two clicks. The site must be fully responsive, ensuring a flawless experience across desktop, tablet, and mobile devices. Fast loading times are non-negotiable, as performance is a direct reflection of our development capabilities.

## 5. AI Generation Prompts & Instructions

To ensure the AI generates the optimal website structure and code, the following instructions should be provided to the AI development tool (e.g., v0, Cursor, or similar platforms):

**System Prompt for AI:**
"You are an expert web developer and UI/UX designer tasked with creating a high-converting portfolio website for a boutique software development agency. The agency specializes in MERN stack development, CMS integration, custom application development, and workflow automation (n8n/Python). The design must be modern, minimalist, and highly professional, utilizing a dark mode aesthetic with vibrant accent colors (e.g., neon blue or electric purple) to convey a cutting-edge technology brand.

**Specific Generation Tasks:**
1.  **Generate the Homepage:** Create a hero section with a strong headline ('Accelerating Business Growth Through Custom Software & Automation'). Include a 'Featured Work' section highlighting three distinct projects (one MERN, one CMS, one Automation). Ensure clear 'Get a Quote' CTAs are visible without scrolling.
2.  **Generate the Case Study Template:** Design a reusable layout for individual portfolio items. This layout must include dedicated sections for the Problem, Solution, Technologies Used (with icons), and Quantifiable Results. Include placeholders for high-resolution screenshots and embedded Loom videos.
3.  **Generate the Services Section:** Create a visually distinct area detailing the four core services. Use interactive elements (like hover effects or accordions) to reveal the specific technologies associated with each service (e.g., hovering over 'MERN Stack' reveals React, Node, MongoDB icons).
4.  **Technical Requirements:** Ensure the generated code is clean, semantic HTML5/CSS3, utilizing a modern framework like Tailwind CSS for styling. The site must be fully responsive and optimized for Core Web Vitals."
