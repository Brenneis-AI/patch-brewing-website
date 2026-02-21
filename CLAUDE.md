# CLAUDE.md

This file provides guidance to Claude Code when working with this repository.

## Project Overview

This is the **Patch Brewing** website. Built and maintained by Brenneis AI.

- **Client:** Patch Brewing
- **Platform:** GoHighLevel (GHL)
- **Stack:** Vanilla HTML, CSS, and JavaScript only
- **No build process, no package manager, no dependencies**

## Deployment Workflow

- HTML and JS together in one section per page — pasted into GHL custom code block
- CSS pasted into individual page Custom CSS setting in GHL
- Global header and footer are GHL global sections
- No global CSS or JS — each page manages its own

## Repository Structure

pages/ — one folder per page
  section-main.html — full HTML and JS for the page
  page.css — page-level CSS
global/
  header.html
  footer.html
CLAUDE.md

## Pages
- home
- menu
- happenings
- private-events

## Conventions

- All files use kebab-case
- Every file must begin with a comment header:

<!--
  File: filename.html
  Page: Which GHL page this belongs to
  Section: What this section does
  Last Updated: YYYY-MM-DD
-->

## Claude Code Behavior Instructions

### Non-Negotiable Rules
- Vanilla HTML, CSS, and JS only
- No external libraries or frameworks
- Always add comment header to every file
- Never create package.json, node_modules, or build files
- JS lives inside section-main.html for this project
- CSS always in page.css — never inline

### Quality Check Before Finishing
- Every file has a comment header
- CSS is in page.css only
- Code is clean and ready to paste into GHL