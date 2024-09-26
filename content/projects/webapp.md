+++
title = "Web App"
slug = "webapp"
+++

## Table of Contents
- [Abstract](#Abstract)
- [Objective](#Objective)
- [Task Breakdown](#task-breakdown)
- [Frontend](#frontend)
- [Backend](#backend)
- [Setup Instructions](#setup-instructions)
- [Thought Process](#thought-process)

## Abstract

This was a takehome project completed in one day to demonstrate my fullstack development abilities. I took the project as a chance to further reinforced what I learned about Next.js and Django on my own.

## Objective
The prompt was to build a web application using Next.js on the frontend and integrate it with a Django API backend. The application will feature a basic dashboard page with multiple charts (Candlestick, Line Chart, Bar Chart, and Pie Chart), and the data will be retrieved from the backend (it can be hardcoded in the backend).

## Task Breakdown

***Frontend: Next.js Application***

Create a basic dashboard page that includes four different types of charts:

- Candlestick Chart

- Line Chart

- Bar Chart

- Pie Chart

Charts Requirement:

- Use a popular charting library such as Chart.js, Rechart, Lightview, or whatever you prefer to implement the charts.

- Each chart should render data that comes from the Django API.

- Next.js Functionality:

- The frontend should fetch the data using Next.js API routes or directly in a React component via a fetch or Axios call.

- Display the fetched data dynamically in the charts.

***Backend: Django API***

Create a simple Django API that provides the data for the charts. The data can be hardcoded for this task.

Define the following API endpoints in Django, each serving data for the respective chart:

- /api/candlestick-data/ – Returns JSON data for the Candlestick chart.

- /api/line-chart-data/ – Returns JSON data for the Line chart.

- /api/bar-chart-data/ – Returns JSON data for the Bar chart.

- /api/pie-chart-data/ – Returns JSON data for the Pie chart.

The data returned from these APIs can be hardcoded but should follow the typical structure that the charts expect.

## Frontend
- **Next.js**: A React framework for server-side rendering and generating static websites.
- **SWR**: A React hook for remote data fetching.
- **Chart.js**: A JavaScript library for creating charts.
- **React Chart.js 2**: A React wrapper for Chart.js.
- **Fetch**: HTTP clients to fetch data from the Django API (depending on your implementation).

## Backend
- **Django**: A Python web framework for building the API.
- **Django REST Framework**: A toolkit to create web APIs in Django.

## Setup Instructions

***Prerequisites***
- Node.js (v14+)
- Python (v3.8+)

***Backend (Django)***

1. **Clone the Repository**:
    git clone https://github.com/takehome.git
    cd takehome/backend

2. **Create a Virtual Environment**:
    python3 -m venv venv
    source venv/bin/activate

3. **Install Dependencies:**:
    pip install -r requirements.txt

4. **Run the Django Server:**:
    python manage.py runserver


5. **Navigate to the Frontend Directory:**:
    cd ../front

6. **Install Dependencies:**:
    npm install

7. **Run the Next.js Development Server:**:
    npm run dev


***Running with Docker (Optional)***
1. Build Docker Image:
    docker-compose up --build

2. Start the Application:
    docker-compose up

3. Start Django server:
    cd takehome/back
    python manage.py runserver


## Thought Process
The approach was to create a simple but robust full-stack application integrating modern frontend and backend technologies:

***Backend:***
I set up the backend first, Django was used for the backend API so I tried to capitalize on its simplicity in creating APIs using the Django REST Framework. The API serves hardcoded chart data which I coded in views.py. There is some remnants of code left from api.py which is a resulted from me learning fullstack coding from online. It's not pretty but it's simple and pretty robust.

***Frontend:***
I then implemented the front end. In this proces I found that I liked working with Next.js even though I had only mostly worked with React, its server-side rendering and react features made it fairly easy to use, though I ended having to do some client side rendering in the end, it's definitely something I could improve on in the future. 

I used SWR for fetching, the page is designed to load the data when it opens, which should be fine for this project. 

For the chart visuals I used Chart.js with React Chart.js and plotly. I used Chart.js for the line, bar, and pie charts, since I had used them before. However I struggled a lot with getting the candlestick chart to work. I first tried using financial charts, but it wouldn't cooperate and I ended up having to use react and plotly, unfortunately making the candlestick graph a bit of an eyesore.

I have looked into using typescript, but I ran into an issue with the fetcher. In the interest of time, I decided to opt for building a Docker for easier integration, as opposed to refactoring the code for typescript. I also did not implement tests or use redux, I will look into how to build those in the future.