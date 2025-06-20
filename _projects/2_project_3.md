---
layout: page
title: Video Streaming DBMS
description: Oracle SQL-based Database System for a YouTube-like Platform
img: assets/img/video_db_schema.jpg
importance: 2
category: Development Projects
related_publications: false
giscus_comments: true
---

# Video Streaming Database System

This project is a **Database Management System (DBMS)** design for a video streaming platform inspired by YouTube. It models the backend data structure and logic using **Oracle SQL**, focusing on key functionalities such as user accounts, video uploads, views, likes, subscriptions, and user history.

---

## 🔍 Project Objective

To design and implement a relational database system that:

- Handles content creation and video uploads
- Tracks user interaction through likes, dislikes, and comments
- Maintains user watch history and subscriptions
- Supports queries for recommendation and analytics

---

## 📊 ER Diagram (Entity-Relationship)

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/video_db_er.jpg" title="ER Diagram" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="caption">
  ER Diagram visualizing the entities (User, Video, History, Likes, Comments, etc.) and their relationships.
</div>

---

## 🧩 Schema Diagram

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/video_db_schema.jpg" title="Schema Diagram" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="caption">
  Schema Diagram showing tables, attributes, data types, primary/foreign keys, and their relationships.
</div>

The schema diagram provides a tabular-level view of the database after transformation from ER to relational format. It outlines:

- All table structures and column definitions
- Primary and foreign key constraints
- Cardinality and referential integrity

---

## 🛠️ Key Features

- ✅ Fully normalized schema
- ✅ User-video interactions (views, likes, comments)
- ✅ Subscriptions and history tracking
- ✅ Analytics queries (top-liked, most-viewed, active users)
- ✅ Views and subqueries for modularity and maintainability

---

## 🧪 Sample SQL Queries

```sql
-- Top 5 most viewed videos
SELECT video_title, view_count
FROM videos
ORDER BY view_count DESC
FETCH FIRST 5 ROWS ONLY;
