# Two-Tier Architecture

A **Two-Tier Architecture** is a system that consists of two separate parts that work together to provide an application. These are the **Web/Application Tier** and the **Database Tier**, where each tier has its own specific function.

## The Web/Application Tier

The Web/Application Tier is responsible for providing the application's interface and responding to requests from users. In this setup, the **Nextcloud container** provides the web application that users access through a web browser. It processes user requests and communicates with the database when information needs to be saved or retrieved.

## The Database Tier

The Database Tier is responsible for storing and managing the application's data. In this setup, the **MariaDB container** stores important information used by Nextcloud, including user accounts, settings, and file-related metadata. It provides the data needed by the application whenever it is requested.

## Why Separate Them?

Keeping the web application and database in separate containers makes the system easier to manage and maintain. Each container can focus on its own purpose, and changes or updates to one service can be made without directly affecting the other service.
