# Bass1in3 - Workout Music Companion
 - Name meaning
   - In music, a bassline is the rhythm foundation that drives a track
   - In workouts, it symbolizes the energy foundation that pushes athletes forward 

### Markdown
This file is called README.md. It is a [Markdown file](https://en.wikipedia.org/wiki/Markdown). Markdown is a simple way to format documents. When a Markdown-ready viewer displays the contents of a file, it formats it to look like HTML. However, Markdown is significantly easier to write than HTML. VSCode supports displaying Markdown in a preview window. GitHub uses Markdown extensively including in every repo's description file, ```README.md```.

All Markdown files end with the extension ```.md```. There is a Markdown tutorial [here](https://www.markdowntutorial.com/) and a Markdown cheatsheet [here](https://www.markdownguide.org/cheat-sheet/).

#### Images
If you would like to add images to a Markdown file, place them in the ```docs/images/``` directory in this repo and reference them using markdown like this:

```
![alt text](relative/path/to/image)
```

Here is how to add the Carthage logo to a Markdown file (you can see the image in the repo right now):

```
![Carthage Firebird Logo](docs/images/firebirdLogo.jpg)
```
![Carthage Firebird Logo](docs/images/firebirdLogo.jpg)

This ensures that images are correctly linked and displayed when viewing the documentation on GitHub or any Markdown-supported platform.

## Code
The ```code``` directory is used to store your code. You can put it all in one directory or you can create subdirectories.

I have added a ```main.cpp``` file to get you started. Feel free to remove it.

If you have any questions feel free to ask me! I'll answer professor questions, customer questions, and give advice if asked.

# Sample Spec

Below is an example of a project specification.  

## Software Requirements Specification for the Mahoney University Registration System

## Introduction

### Purpose
The purpose of this document is to outline the functional and non-functional requirements of Mahoney University’s new online registration system. The system is designed to streamline the registration process for students and faculty, replacing the outdated manual system. This specification serves as a contract between the system stakeholders and the developers to ensure that the system meets the needs of its users while adhering to university policies and technical constraints.

The key goals of the new system are:
- To improve the efficiency of the course registration process for students.
- To provide staff in the Registrar’s Office with tools to manage course offerings, schedules, and student records.
- To enhance the accuracy and accessibility of student academic information, such as grades and enrollment history.
- To support the university’s transition to digital infrastructure while maintaining compatibility with legacy systems during a transitional period.

### Scope
This system is intended to support the registration process for all students at Mahoney University, including undergraduates, graduate students, and non-degree-seeking students. The system will handle:
- Student authentication and secure access to personal records.
- Course search and registration.
- Enrollment validation, including prerequisite checks and course availability.
- Management of student schedules, including the ability to add, drop, or modify course enrollments.
- Grade viewing and transcript requests.

The scope of the system also includes administrative tools for the Registrar’s Office to:
- Create and modify course offerings for each academic term.
- Manage enrollment caps, waitlists, and course prerequisites.
- Track student progress and generate reports for academic performance.

### Definitions, Acronyms, and Abbreviations
- **Registrar**: The official responsible for maintaining student records, managing course schedules, and overseeing the registration process.
- **Student Information System (SIS)**: A university-wide database that stores student records, course information, and academic data.
- **GPA**: Grade Point Average, a numerical representation of a student's academic performance.
- **Semester**: A division of the academic year, typically consisting of a Fall and Spring term, in which courses are offered and completed.
- **Waitlist**: A system that allows students to reserve a spot in a full course, subject to availability if another student drops the course.
- **Prerequisite**: A course or requirement that must be completed before a student can enroll in a more advanced course.
- **User Role**: A designation for system access levels, such as student, registrar, or faculty member, each with different permissions within the system.
- **Concurrent Enrollment**: The ability for students to be enrolled in multiple courses during the same academic term.

## Overview
The Mahoney University Registration System is a web-based platform designed to automate the course registration process for students and faculty. It serves as the primary interface for students to manage their academic schedules and for university staff to oversee the course offerings and registration workflows.

### System Features:
1. **Secure Login**: Ensures that only authorized users (students, faculty, and staff) have access to the system, with user authentication based on university credentials.
2. **Course Search**: Allows students to browse available courses by department, term, and subject, with filtering options based on course availability, schedule, and prerequisites.
3. **Course Registration**: Students can add or drop courses, view class schedules, and receive notifications of any conflicts or unmet prerequisites.
4. **Grades and Transcripts**: Provides students with access to their grades from current and past semesters, as well as the ability to request official transcripts.
5. **Registrar Management Tools**: The Registrar’s Office can create, modify, and delete course sections, set enrollment limits, and manage waitlists.

The system is designed with scalability in mind, allowing it to handle thousands of students registering simultaneously during peak periods. It will integrate with the university’s existing Student Information System (SIS) and is built using modern web technologies to ensure ease of use, reliability, and performance.

The following sections detail the specific use cases that the system will support, describing how students and staff will interact with the system during typical operations.

## Use Cases

### Use Case 1 - Library Exploration (End User)
	-  Browse Catalog
		•	Action: Scroll grid/rail of tiles with thumbnails, titles, energy badges.
		•	Goal: Discover songs visually without forms.
	- Search & Filter
		•	Action: Search by title; filter by tags (Warmup/HIIT/Cooldown/etc.) or energy ranges.
		•	Goal: Quickly narrow to what fits today’s workout.
	- Tag Quick Picks
		•	Action: Tap tag chips (e.g., “Hype”, “Recovery”) to view pre-filtered sets.
		•	Goal: One-tap curation.


### Use Case 2  - Interactive Workout Building (End User)
	- Drag-and-Drop Rail
		•	Action: Drag tiles from the library onto a horizontal timeline; color/label segments (Warmup, Push, Recover).
		•	Goal: Compose a session playfully.
	- Card Stack Suggestions
		•	Action: Swipe right to add, left to skip, up to star; suggestions respect current filters (tags/energy).
		•	Goal: Rapid assembly without browsing.
	- Quick Draft (Auto)
		•	Action: Pick a feeling  (“Leg Day”, “Morning Run”) → app drafts a session from the preloaded catalog.
		•	Goal: 10-second start.
	- Challenge Modes (May not do just a idea )
		•	Action: Tabata/Pyramid/Countdown generators pick from the catalog by tag/energy rules.
		•	Goal: Fun, structured workouts without manual picking.
	- Reorder & Replace
		•	Action: Drag to reorder; tap a tile to cycle through 2–3 similar alternatives from the catalog.
		•	Goal: Fine-tune flow quickly.
	- Save as Template
		•	Action: Save the current rail layout for reuse.
		•	Goal: Build personal routines.


### Use Case 3 Playback 
	- Start Session
		•	Action: Press Play → mini player appears; tap to expand to full player video.
		•	Goal: Seamless start.
	- Queue Sheet (“Up Next”)
		•	Action: Pull up sheet to view/reorder remaining tiles; swipe to remove; add suggestions at the end.
		•	Goal: Mid-workout control.
	- Transport Controls
		•	Action: Play/Pause, Next/Previous, scrub with haptic ticks.
		•	Goal: Core playback UX.
	- Re-roll Next / Boost
		•	Action: Swap the upcoming/current song with a similar/higher-energy pick from the catalog.
		•	Goal: Keep momentum aligned with effort.
	- Audio-only / PiP / AirPlay
		•	Action: Toggle video→audio, enable Picture-in-Picture, route to speakers.
		•	Goal: Flexibility for battery, multitasking, and gyms.



### Use Case 4 Athlete-Focused Enhancements
	- Segment Timer Ring & Toasts
		•	Action: See countdown overlay and “Next segment” toast ~10s before change.
		•	Goal: Stay in the zone.
	- Shake to Reshuffle
		•	Action: Shake to reshuffle remaining queue within current tag/energy constraints.
		•	Goal: Fast rescue if vibe is off.
	- Hype Tap
		•	Action: Double-tap to mark a hype moment (visual pulse + log).
		•	Goal: Capture motivation spikes.
	- Low-Distraction Mode
		•	Action: Dim UI, keep only progress/timer.
		•	Goal: Focus during tough sets.


### Use Case 5 Post-Workout 
	- Recap Timeline
		•	Action: View colored rail of what played, skips, hypes, boosts.
		•	Goal: Reflection & learning.
	- Save as Template from Recap
		•	Action: One-tap to save the completed flow.
		•	Goal: Turn a good session into a repeatable plan.
	- Quick Edit & Re-save
		•	Action: Long-press any segment to replace from similar picks; save v2.
		•	Goal: Iterate over time.

### Use Case 6System & Edge Cases
	- Ad Handling
		•	Behavior: Show “Ad playing” placeholder with countdown; allow skip to next catalog item.
		•	Goal: Maintain rhythm.
	- Unavailable Video Fallback
		•	Behavior: If a video is blocked/removed, auto-skip to the nearest match by tag/energy; log incident.
		•	Goal: Smooth continuity.
	- Lock Screen & Background
		•	Behavior: Media controls + artwork on lock screen; continue audio when screen locks.
		•	Goal: Real workout usability.
