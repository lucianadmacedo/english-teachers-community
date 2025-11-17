# English Teachers Study Groups Platform

A community-based platform for English teachers to form collaborative study groups based on their English proficiency levels.

## Overview

This platform creates small study groups (max 5 people) where English teachers can learn together, share experiences, and support each other's professional development. Advanced speakers (C1-C2) serve as mentors for groups of learners at lower levels.

## How It Works

### 1. Level Selection
Teachers scan a QR code (or visit the website) and select their English level:
- **C1-C2 (Advanced)** - Proficient speakers
- **B2 (Upper Intermediate)** - Independent users
- **B1 (Pre-Intermediate)** - Threshold level
- **A1-A2 (Elementary)** - Basic users

### 2. Registration
Users provide:
- Full name
- Email
- Institution (optional)
- Learning goals

### 3. Automatic Group Assignment

**For C1-C2 Level (Mentors):**
- Assigned as mentors to groups of lower-level learners
- Each mentor guides one study group
- Priority given to groups without mentors

**For Other Levels:**
- Placed in groups with others at the same level
- Maximum 5 members per group
- Each group gets a C1-C2 mentor when available

### 4. Dashboards

**Mentor Dashboard:**
- Pedagogy training tasks (5 modules on teaching English to adults)
- View group members
- Access to resources
- Track training progress

**Learner Dashboard:**
- Level-appropriate learning tasks (5 tasks per level)
- View study group and mentor
- Progress tracking
- Access to resources and support

### 5. Group Page
- See all group members and their goals
- View mentor information
- Ask for help from the group
- Access shared resources
- Community support features

## Features

✅ **Smart Group Assignment**
- Automatic matching based on level
- Maximum 5 people per group
- C1-C2 speakers become mentors

✅ **Differentiated Task Lists**
- Mentors: Pedagogy and teaching methodology
- A1-A2: Basic grammar, vocabulary, simple communication
- B1: Intermediate structures, academic language
- B2: Advanced grammar, idiomatic expressions, discussion leading

✅ **Progress Tracking**
- Visual progress bars
- Task completion checkboxes
- Personal achievement tracking

✅ **Community Building**
- Group member profiles
- Shared goals and experiences
- Support requests
- Resource sharing

## File Structure

```
english-teachers-community/
├── index.html              # Landing page - Level selection
├── register.html           # Registration and group assignment
├── mentor-dashboard.html   # Dashboard for C1-C2 mentors
├── learner-dashboard.html  # Dashboard for learners
├── group.html             # Group page for collaboration
└── README.md              # This file
```

## Technical Details

**Technology Stack:**
- Pure HTML/CSS/JavaScript (no frameworks)
- localStorage for data persistence
- Mobile-responsive design
- QR code compatible

**Data Storage:**
- User data: localStorage
- Groups: localStorage
- Task completion: localStorage

**Note:** This is a client-side prototype. For production use, replace localStorage with a proper backend (Firebase, Supabase, etc.)

## Usage

### For Conference Organizers

1. Host these files on a web server or GitHub Pages
2. Generate a QR code pointing to the index.html URL
3. Display QR code at conference
4. Participants scan and join their groups

### For Development/Testing

1. Open `index.html` in a web browser
2. Select a level and register
3. Complete the flow to see the appropriate dashboard
4. Open in multiple browser tabs to simulate multiple users

## Customization

### Adding More Levels
Edit the level buttons in `index.html` and add corresponding task sets in `learner-dashboard.html`

### Changing Tasks
Modify the task arrays in:
- `mentor-dashboard.html` - Line 238 (mentorTasks array)
- `learner-dashboard.html` - Lines 228-286 (learningTasks object)

### Adjusting Group Size
Change the maximum members check in `register.html`:
- Line 115: `g.members.length < 5` (change 5 to desired size)

### Styling
All CSS is embedded in each HTML file's `<style>` section for easy customization

## Future Enhancements

- Backend database integration
- Real-time chat/messaging
- File sharing for resources
- Calendar/meeting scheduling
- Video call integration
- Email notifications
- Admin panel for organizers
- Analytics and reporting

## Support

This platform is designed to foster a supportive community where teachers can:
- Learn from peers at their level
- Receive guidance from advanced mentors
- Share teaching experiences
- Access curated resources
- Ask questions and get help

---

Built with the goal of creating a collaborative, supportive community of English teachers committed to professional growth.
