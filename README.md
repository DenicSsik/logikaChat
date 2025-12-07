# CTk Chat Client

A lightweight chat client built with **CustomTkinter**, featuring a
sliding side menu, adaptive UI layout, and real-time messaging through
TCP sockets.

## ✨ Features

-   📡 **Real-time messaging** using Python sockets\
-   🎨 **CustomTkinter interface** with modern UI components\
-   📁 **Sliding menu panel** with smooth animation\
-   🔄 **Fully adaptive layout** --- automatically adjusts to window
    size\
-   🧵 **Multithreaded message listener** (non-blocking UI)\
-   💬 **Scrollable chat panel** for readable message history

## 🚀 How It Works

-   On startup, the client connects to `localhost:8080`
-   Sends a "joined the chat" notice
-   Listens for messages on a separate daemon thread\
-   Displays new messages instantly\
-   The menu button toggles a smooth sliding animation\
-   UI elements auto-resize every 10 ms for perfect layout

## 📦 Requirements

    customtkinter

## ▶️ Launching

    python logikaTalk.py

## 🧩 File Overview

-   `MainWindow` --- main app class\
-   `show_menu()` --- controls sliding menu\
-   `menu_anim()` --- smooth animation loop\
-   `send_message()` --- sends user input to server\
-   `get_messages()` --- listens for incoming messages\
-   `adaptive_ui()` --- dynamically updates layout

## 🖼 UI Features

-   Side menu with dynamic width\
-   Chat field with auto-expanding scroll area\
-   Entry box for writing messages\
-   Animated button toggling the menu\
-   Username input (inside menu)

## ⚠️ Notes

This client assumes a simple TCP chat server implementation.
