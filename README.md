<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>

    <link rel="stylesheet" href="ind2.css">

</head>

<body>

    <nav id="sidebar">
        <ul>
            <li>
                <span class="logo">coding2go</span>
                <button onclick=toggleSidebar() id="toggle-btn">
          <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px" fill="#e8eaed"><path d="m313-480 155 156q11 11 11.5 27.5T468-268q-11 11-28 11t-28-11L228-452q-6-6-8.5-13t-2.5-15q0-8 2.5-15t8.5-13l184-184q11-11 27.5-11.5T468-692q11 11 11 28t-11 28L313-480Zm264 0 155 156q11 11 11.5 27.5T732-268q-11 11-28 11t-28-11L492-452q-6-6-8.5-13t-2.5-15q0-8 2.5-15t8.5-13l184-184q11-11 27.5-11.5T732-692q11 11 11 28t-11 28L577-480Z"/></svg>
        </button>
            </li>
            <li class="active">
                <a href="index.html">
                    <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px" fill="#e8eaed"><path d="M240-200h120v-200q0-17 11.5-28.5T400-440h160q17 0 28.5 11.5T600-400v200h120v-360L480-740 240-560v360Zm-80 0v-360q0-19 8.5-36t23.5-28l240-180q21-16 48-16t48 16l240 180q15 11 23.5 28t8.5 36v360q0 33-23.5 56.5T720-120H560q-17 0-28.5-11.5T520-160v-200h-80v200q0 17-11.5 28.5T400-120H240q-33 0-56.5-23.5T160-200Zm320-270Z"/></svg>
                    <span>Home</span>
                </a>
            </li>
            <li>
                <a href="dashboard.html">
                    <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px" fill="#e8eaed"><path d="M520-640v-160q0-17 11.5-28.5T560-840h240q17 0 28.5 11.5T840-800v160q0 17-11.5 28.5T800-600H560q-17 0-28.5-11.5T520-640ZM120-480v-320q0-17 11.5-28.5T160-840h240q17 0 28.5 11.5T440-800v320q0 17-11.5 28.5T400-440H160q-17 0-28.5-11.5T120-480Zm400 320v-320q0-17 11.5-28.5T560-520h240q17 0 28.5 11.5T840-480v320q0 17-11.5 28.5T800-120H560q-17 0-28.5-11.5T520-160Zm-400 0v-160q0-17 11.5-28.5T160-360h240q17 0 28.5 11.5T440-320v160q0 17-11.5 28.5T400-120H160q-17 0-28.5-11.5T120-160Zm80-360h160v-240H200v240Zm400 320h160v-240H600v240Zm0-480h160v-80H600v80ZM200-200h160v-80H200v80Zm160-320Zm240-160Zm0 240ZM360-280Z"/></svg>
                    <span>Dashboard</span>
                </a>
            </li>
            <li>
                <button onclick=toggleSubMenu(this) class="dropdown-btn">
          <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px" fill="#e8eaed"><path d="M160-160q-33 0-56.5-23.5T80-240v-480q0-33 23.5-56.5T160-800h207q16 0 30.5 6t25.5 17l57 57h320q33 0 56.5 23.5T880-640v400q0 33-23.5 56.5T800-160H160Zm0-80h640v-400H447l-80-80H160v480Zm0 0v-480 480Zm400-160v40q0 17 11.5 28.5T600-320q17 0 28.5-11.5T640-360v-40h40q17 0 28.5-11.5T720-440q0-17-11.5-28.5T680-480h-40v-40q0-17-11.5-28.5T600-560q-17 0-28.5 11.5T560-520v40h-40q-17 0-28.5 11.5T480-440q0 17 11.5 28.5T520-400h40Z"/></svg>
          <span>Create</span>
          <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px" fill="#e8eaed"><path d="M480-361q-8 0-15-2.5t-13-8.5L268-556q-11-11-11-28t11-28q11-11 28-11t28 11l156 156 156-156q11-11 28-11t28 11q11 11 11 28t-11 28L508-372q-6 6-13 8.5t-15 2.5Z"/></svg>
        </button>
                <ul class="sub-menu">
                    <div>
                        <li><a href="#">Folder</a></li>
                        <li><a href="#">Document</a></li>
                        <li><a href="#">Project</a></li>
                    </div>
                </ul>
            </li>
            <li>
                <button onclick=toggleSubMenu(this) class="dropdown-btn">
          <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px" fill="#e8eaed"><path d="m221-313 142-142q12-12 28-11.5t28 12.5q11 12 11 28t-11 28L250-228q-12 12-28 12t-28-12l-86-86q-11-11-11-28t11-28q11-11 28-11t28 11l57 57Zm0-320 142-142q12-12 28-11.5t28 12.5q11 12 11 28t-11 28L250-548q-12 12-28 12t-28-12l-86-86q-11-11-11-28t11-28q11-11 28-11t28 11l57 57Zm339 353q-17 0-28.5-11.5T520-320q0-17 11.5-28.5T560-360h280q17 0 28.5 11.5T880-320q0 17-11.5 28.5T840-280H560Zm0-320q-17 0-28.5-11.5T520-640q0-17 11.5-28.5T560-680h280q17 0 28.5 11.5T880-640q0 17-11.5 28.5T840-600H560Z"/></svg>
          <span>Todo-Lists</span>
          <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px" fill="#e8eaed"><path d="M480-361q-8 0-15-2.5t-13-8.5L268-556q-11-11-11-28t11-28q11-11 28-11t28 11l156 156 156-156q11-11 28-11t28 11q11 11 11 28t-11 28L508-372q-6 6-13 8.5t-15 2.5Z"/></svg>
        </button>
                <ul class="sub-menu">
                    <div>
                        <li><a href="#">Work</a></li>
                        <li><a href="#">Private</a></li>
                        <li><a href="#">Coding</a></li>
                        <li><a href="#">Gardening</a></li>
                        <li><a href="#">School</a></li>
                    </div>
                </ul>
            </li>
            <li>
                <a href="calendar.html">
z          <span>Calendar</span>
        </a>
            </li>
            <li>
                <a href="profile.html">
                    <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px" fill="#e8eaed"><path d="M480-480q-66 0-113-47t-47-113q0-66 47-113t113-47q66 0 113 47t47 113q0 66-47 113t-113 47ZM160-240v-32q0-34 17.5-62.5T224-378q62-31 126-46.5T480-440q66 0 130 15.5T736-378q29 15 46.5 43.5T800-272v32q0 33-23.5 56.5T720-160H240q-33 0-56.5-23.5T160-240Zm80 0h480v-32q0-11-5.5-20T700-306q-54-27-109-40.5T480-360q-56 0-111 13.5T260-306q-9 5-14.5 14t-5.5 20v32Zm240-320q33 0 56.5-23.5T560-640q0-33-23.5-56.5T480-720q-33 0-56.5 23.5T400-640q0 33 23.5 56.5T480-560Zm0-80Zm0 400Z"/></svg>
                    <span>Profile</span>
                </a>
            </li>
        </ul>
    </nav>

    <main>
        <div class="container">
            <h1>Heading</h1>
            <p>This is a paragraph of text that provides information about the topic at hand. It is meant to be informative and engaging for the reader.</p>
        </div>
        <div class="container">
            <h1>Heading</h1>
            <p>This is a paragraph of text that provides information about the topic at hand. It is meant to be informative and engaging for the reader.</p>
        </div>

        <div class="container">
            <h1>Heading</h1>
            <p>This is a paragraph of text that provides information about the topic at hand. It is meant to be informative and engaging for the reader.</p>
        </div>
    </main>
</body>

</html>

@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
:root {
    --base-clr: #11121a;
    --line-clr: #42434a;
    --hover-clr: #222533;
    --text-clr: #e6e6ef;
    --accent-clr: #5e63ff;
    --secondary-text-clr: #b0b3c1;
}

* {
    margin: 0;
    padding: 0;
}

html {
    font-family: Poppins, 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.5rem;
}

body {
    min-height: 100vh;
    min-height: 100dvh;
    background-color: var(--base-clr);
    color: var(--text-clr);
    display: grid;
    grid-template-columns: auto 1fr;
}

#sidebar {
    box-sizing: border-box;
    height: 100vh;
    width: 250px;
    padding: 5px 1em;
    background-color: var(--base-clr);
    border-right: 1px solid var(--line-clr);
    position: sticky;
    top: 0;
    align-self: start;
    transition: 300ms ease-in-out;
    overflow: hidden;
    text-wrap: nowrap;
}

#sidebar.close {
    padding: 5px;
    width: 60px;
}

#sidebar ul {
    list-style: none;
}

#sidebar>ul>li:first-child {
    display: flex;
    justify-content: flex-end;
    margin-bottom: 16px;
    .logo {
        font-weight: 600;
    }
}

#sidebar ul li.active a {
    color: var(--accent-clr);
    svg {
        fill: var(--accent-clr);
    }
}

#sidebar a,
#sidebar .dropdown-btn,
#sidebar .logo {
    border-radius: .5em;
    padding: .85em;
    text-decoration: none;
    color: var(--text-clr);
    display: flex;
    align-items: center;
    gap: 1em;
}

.dropdown-btn {
    width: 100%;
    text-align: left;
    background: none;
    border: none;
    font: inherit;
    cursor: pointer;
}

#sidebar svg {
    flex-shrink: 0;
    fill: var(--text-clr);
}

#sidebar a span,
#sidebar .dropdown-btn span {
    flex-grow: 1;
}

#sidebar a:hover,
#sidebar .dropdown-btn:hover {
    background-color: var(--hover-clr);
}

#sidebar .sub-menu {
    display: grid;
    grid-template-rows: 0fr;
    transition: 300ms ease-in-out;
    >div {
        overflow: hidden;
    }
}

#sidebar .sub-menu.show {
    grid-template-rows: 1fr;
}

.dropdown-btn svg {
    transition: 200ms ease;
}

.rotate svg:last-child {
    rotate: 180deg;
}

#sidebar .sub-menu a {
    padding-left: 2em;
}

#toggle-btn {
    margin-left: auto;
    padding: 1em;
    border: none;
    border-radius: .5em;
    background: none;
    cursor: pointer;
    svg {
        transition: rotate 150ms ease;
    }
}

#toggle-btn:hover {
    background-color: var(--hover-clr);
}

main {
    padding: min(30px, 7%);
}

main p {
    color: var(--secondary-text-clr);
    margin-top: 5px;
    margin-bottom: 15px;
}

.container {
    border: 1px solid var(--line-clr);
    border-radius: 1em;
    margin-bottom: 20px;
    padding: min(3em, 15%);
    h2,
    p {
        margin-top: 1em
    }
}

@media(max-width: 800px) {
    body {
        grid-template-columns: 1fr;
    }
    main {
        padding: 2em 1em 60px 1em;
    }
    .container {
        border: none;
        padding: 0;
    }
    #sidebar {
        height: 60px;
        width: 100%;
        border-right: none;
        border-top: 1px solid var(--line-clr);
        padding: 0;
        position: fixed;
        top: unset;
        bottom: 0;
        >ul {
            padding: 0;
            display: grid;
            grid-auto-columns: 60px;
            grid-auto-flow: column;
            align-items: center;
            overflow-x: scroll;
        }
        ul li {
            height: 100%;
        }
        ul a,
        ul .dropdown-btn {
            width: 60px;
            height: 60px;
            padding: 0;
            border-radius: 0;
            justify-content: center;
        }
        ul li span,
        ul li:first-child,
        .dropdown-btn svg:last-child {
            display: none;
        }
        ul li .sub-menu.show {
            position: fixed;
            bottom: 60px;
            left: 0;
            box-sizing: border-box;
            height: 60px;
            width: 100%;
            background-color: var(--hover-clr);
            border-top: 1px solid var(--line-clr);
            display: flex;
            justify-content: center;
            >div {
                overflow-x: auto;
            }
            li {
                display: inline-flex;
            }
            a {
                box-sizing: border-box;
                padding: 1em;
                width: auto;
                justify-content: center;
            }
        }
    }
}
