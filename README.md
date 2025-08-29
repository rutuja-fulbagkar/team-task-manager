
###  Project Name
A full-featured frontend application with authentication (including OTP email verification), advanced task/project management (Kanban board), dynamic filtering, export capabilities, robust form validations, and more—all built with React, Material UI, and a modern state management stack.

### Project setup
```
npm install
```

#### Compiles and hot-reloads for development
```
npm run dev
```

#### Compiles and minifies for production
```
npm run build
```

🌟 Features Overview
Authentication
Secure login and registration, with OTP verification via email for signup and password reset.

Project & Task Management
Manage projects and tasks in a visually interactive Kanban board built with @hello-pangea/dnd and Material UI.

Advanced Filtering & Search
Real-time filtering and search for projects and tasks, including filters by status, assignee, and due date.

Dynamic Pagination
Paginated lists for efficient browsing of large datasets with customizable page size.

Conditional Rendering
Contextual display of components, statuses, and actions (e.g., only project owners can add members, task access restricted to project members).

Data Export
Export data to CSV/XLSX and support for screenshot/pdf export via html2canvas and file-saver.

Form Validation
All forms are validated using Yup and react-hook-form for robust UX.

Material UI Integration
Modern UI with @mui/material and @mui/icons-material, fully responsive styles, and custom themes.

Activity Logs & Notifications
Real-time task/project activity logs and visual timeline; users receive in-app feedback via react-toastify.

File Uploads & Attachments
Upload, preview, and manage files directly within tasks or projects.

Charts and Analytics
Task/project analytics visualized using chart.js.

🛠 Technologies & Dependencies
Major dependencies:

React 19, React Router 7, Redux Toolkit, Redux Persist, React Redux

Material UI (MUI), @mui/lab, @mui/x-date-pickers

Tailwind CSS (optional), styled-components

react-hook-form, @hookform/resolvers, yup (form validation)

@hello-pangea/dnd (Kanban drag-and-drop)

date-fns, dayjs, moment

lodash, clsx

chart.js

xlsx, file-saver, html2canvas (export utilities)

react-icons / @mui/icons-material

axios

📝 Assumptions and Decisions
Only project owners can add/remove members; access is role-based.

All authentication and user-sensitive operations are protected with JWT tokens.

Task and project Kanban are available to members of each project only.

Email-based OTP is required for verification and password reset flows.

Application follows a strict separation between presentational and logic components for maintainability.

All state is managed with Redux Toolkit and persisted for smooth UX.

