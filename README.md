# Hi, I'm Nicolás Bazaes

I'm a developer and Linux enthusiast based in Los Ángeles, Chile. I build web applications, automate repetitive tasks, and run my own servers. Backend development and system administration are the parts I keep coming back to, though I enjoy building the interface people actually use, too.

Most of my projects start with something close to home: a business workflow, a scheduling problem in my community, or a tool I'd like to have on my own computer. That has taken me from Django and React applications to Android apps, desktop tools, and a small contribution to the Linux kernel.

## Things I've built

### [BazPOS](https://github.com/nbazaes/django-bazpos)

A point-of-sale and business management application covering sales, inventory, suppliers, invoices, returns, and cash register closing. It brings everyday store operations into one place, with access controlled by user roles.

React handles the interface, Django REST Framework handles the API and business logic, and MariaDB stores the data. The deployment uses Docker Compose, Gunicorn, and nginx. It's the clearest example of how I work across the application and the infrastructure underneath it.

### [MarkIt Desktop](https://github.com/nbazaes/markit-desktop)

A desktop interface for Microsoft's MarkItDown file-to-Markdown converter, built with Tauri, Svelte, and a Python conversion backend. It adds drag-and-drop input, batch conversion, and a preview so documents can be converted without working through the command line.

This project is also an experiment in building desktop applications with a web interface and a native shell.

### [Discursantes](https://github.com/nbazaes/discursantes_react)

A React application for organizing Sunday speakers in a local congregation. It replaces paper and spreadsheets with a shared place for assignments, dates, topics, and speaking history. A practical project shaped by a need in my own community.

### [FamilyApp](https://github.com/nbazaes/family-app)

A self-hosted family organizer with shared shopping lists, tasks, calendars, and expense tracking. The Android client uses Kotlin and Jetpack Compose, with local storage and background synchronization against a FastAPI backend.

It's where I explore keeping everyday tools useful when the connection isn't available, while retaining control over where the data lives.

I've also built a [Python tool for downloading received invoices from Chile's SII](https://github.com/nbazaes/descargar-facturas-sii) and [TicketOps AI](https://github.com/nbazaes/ticketops-ai), an experiment in turning technical support reports into structured classifications with FastAPI, Astro, and local language models.

## A small fix upstream

I contributed a Synaptics driver change that enables automatic SMBus/RMI4 selection for the ThinkPad E490's touchpad. The patch was merged into the Linux kernel and backported to stable branches.

The [contribution record](https://github.com/nbazaes/linux-kernel-patches) documents the hardware testing, review process, and release availability, with a link to the [upstream commit](https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/commit/?id=16ca52bc209fa4bf9239cd9e5643e95533476b58).

## Tools I work with

- **Backend & data:** Python, Django, Django REST Framework, FastAPI, Node.js, SQL, MariaDB, PostgreSQL, SQLite.
- **Interfaces:** React, Astro, JavaScript, TypeScript; Svelte and Tauri for desktop experiments, Kotlin and Jetpack Compose for Android.
- **Infrastructure:** Linux, Bash, Docker Compose, nginx, and self-hosted services.

## Say hello

I'm happy to talk about development opportunities, a project you need help with, or Linux and self-hosting. You can explore my [personal website](https://nbazaes.dev), including its interactive terminal, or reach me at [nbazaes@bazaes.cl](mailto:nbazaes@bazaes.cl).
