# vision_agent
Vision Agent: An AI-Powered Web Automation Framework Using Vision Language Models

Team


Bomma Jeshwanth Goud — 23AG1A0577

Vuddamarri Ashwitha — 23AG1A05C8

Pabbathi Varun Sai — 23AG1A05A6


Guide: Mr. A. Ramesh, Associate Professor


Abstract

Vision Agent is an AI-powered web automation framework designed to browse and interact with web pages like a human. Traditional automation tools often depend on fixed scripts and can break when a website changes its layout. Vision Agent addresses this problem by using screenshots, visual elements, and a Vision Language Model (VLM) to decide what action should be performed.


The system captures web pages, adds numbered tags to interactive elements such as buttons and text boxes, and enables the AI agent to decide whether to click, type, scroll, or navigate. It also includes self-checking, human-help fallback, and detailed action logging for reliable and transparent automation.


Problem Statement

Traditional web automation tools have several limitations:



Fixed automation scripts can break when website layouts change.

Developers spend significant time maintaining and updating broken scripts.

Text-only automation struggles with visual elements such as calendars, pop-ups, maps, and shopping carts.

There is a need for adaptive AI that can visually understand and navigate dynamic web pages.


Objectives


Build a human-like web agent that can understand web pages using screenshots and text.

Enable precise clicking and typing through numbered visual labels.

Automate real-world multi-step tasks such as online shopping, flight booking, and form filling.

Provide safety and transparency through self-checking, human assistance, and step-by-step action logs.


Literature Survey

The project is based on the research paper:


WebVoyager: Building an End-to-End Web Agent with Large Multimodal Models — He et al. (2024).


The referenced work demonstrates the use of visual screenshots and text for web agents and reports a 59.1% success rate on real websites compared with 40.1% for older text-only agents.


Vision Agent extends this direction by focusing on a complete software system using Spring Boot, React, Playwright, self-checking, human support fallback, and detailed action logging for practical web automation.


System Workflow


Browser Control Setup — Playwright is connected with Spring Boot to control the browser.

Screen Capture & Tagging — The system captures a web-page screenshot and adds numbered tags to interactive elements.

AI Decision Making — The tagged screenshot is provided to the Vision AI, which determines the next action.

Action Execution — The selected click, typing, scrolling, or navigation action is executed in the browser.

Self-Check & Human Help — The system verifies whether the action succeeded and requests human assistance when confidence is low.

Trace Logging — Screenshots and actions are recorded so the process can be reviewed.


Functional Requirements


Capture web-page screenshots and text in real time.

Add numbered visual markers to buttons and text boxes.

Automatically click, type, scroll, and navigate.

Perform self-checks after actions.

Request human assistance when required.

Store action history and logs.


Non-Functional Requirements


Adaptability: Handle changes in website layouts.

Performance & Safety: Use Redis caching for efficient operation and protect user privacy.


Technology Stack

Category	Technology
Programming Languages	Java, JavaScript, SQL
Backend	Spring Boot
Frontend	React
Browser Automation	Playwright
Database	PostgreSQL
Caching	Redis
Containerization	Docker
AI	Vision Language Model (VLM) API

Hardware Requirements


Computer/Laptop

Minimum 8 GB RAM

Multi-core processor


Key Features


Vision-based web-page understanding

Numbered visual element tagging

Automated browser interaction

Multi-step task execution

Self-checking mechanisms

Human-in-the-loop fallback

Detailed action and screenshot logging

Adaptation to changing website layouts


Expected Applications

The framework is designed for practical browser-based tasks such as:



Online shopping

Flight booking

Form filling

Web navigation

Other multi-step web automation workflows


Conclusion

Vision Agent proposes an AI-driven approach to web automation that combines visual page perception with browser control. Instead of depending entirely on fixed scripts, the system can perceive page layouts, adapt to dynamic websites, execute actions, verify results, and maintain a trace of the automation process.


The project aims to bridge the gap between traditional static automation scripts and practical, adaptable AI web agents.


Project Status

The project is presented as a research-oriented software framework and is being developed using Spring Boot, React, Playwright, PostgreSQL, Redis, Docker, and a Vision Language Model API.


Team Members

Bomma Jeshwanth Goud — 23AG1A0577
Vuddamarri Ashwitha — 23AG1A05C8
Pabbathi Varun Sai — 23AG1A05A6

