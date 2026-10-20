# Student Queue Management System

A simple, responsive website demonstrating the **queue** data structure using HTML, CSS, and JavaScript.

## Features

- Register students with their name and student ID
- Automatically generate queue numbers
- Display the waiting list and number of waiting students
- Call the next student using FIFO (First In, First Out)
- Mark the current student as served
- Display currently serving and total students served
- Save queue data in the browser using `localStorage`
- Responsive layout for desktop and mobile screens

## Files

- `index.html` — the complete website (HTML, CSS, and JavaScript)

## Run the website locally

1. Download or clone this repository.
2. Open `index.html` in a web browser.
3. Add test students, click **Call Next Student**, and then click **Mark as Served**.

## Publish with GitHub Pages

1. Create a public repository on GitHub, for example `student-queue-management`.
2. Upload `index.html` and `README.md` to the top-level (root) of the repository.
3. Open the repository's **Settings**.
4. Select **Pages** under **Code and automation**.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Choose the `main` branch and the `/(root)` folder, then click **Save**.
7. Wait for deployment and use the **Visit site** link shown in the Pages settings.

Your website URL will look like:

`https://YOUR-USERNAME.github.io/student-queue-management/`

Replace `YOUR-USERNAME` with your GitHub username.

## How the queue works

This project follows **FIFO (First In, First Out)**:

- **Enqueue:** `queue.push(student)` adds a student to the end.
- **Dequeue:** `queue.shift()` removes the first student from the waiting queue.
- **Front/current student:** `currentStudent` stores the student currently being served.

## Important limitations

This is a learning/demo project. `localStorage` only saves data in the current browser on the current device. It does not synchronize multiple users or computers. Do not use real sensitive student information in a public demo. A production system would need secure authentication, a backend, and a shared database.

## Technologies

- HTML5
- CSS3
- JavaScript
- Browser `localStorage`
- GitHub Pages
