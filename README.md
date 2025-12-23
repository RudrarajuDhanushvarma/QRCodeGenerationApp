# Spring Boot QR Code Generator

A simple and efficient web application to generate QR codes from URLs. This project uses **Spring Boot** for the backend logic and **Google ZXing** for the image encoding process, paired with a clean HTML/CSS frontend.

## 🚀 Features

* **URL Encoding**: Converts any text or URL into a standard QR code.
* **Custom Sizing**: Allows users to specify the width and height of the generated QR code.
* **Instant Preview**: Returns the QR code as a PNG image directly to the browser.
* **Simple Integration**: Uses standard form-urlencoded data for easy frontend-to-backend communication.

## 🛠️ Technology Stack

* **Backend**: Java 17+, Spring Boot
* **QR Logic**: Google ZXing (Zebra Crossing)
* **Frontend**: HTML5, CSS3
* **Logging**: SLF4J for tracking generation requests

## 📋 API Reference

### Generate QR Code

**Endpoint:** `POST /generate`  
**Consumes:** `application/x-www-form-urlencoded`

| Parameter | Type | Default | Description |
| :--- | :--- | :--- | :--- |
| `url` | `String` | Required | The content to encode in the QR code. |
| `size` | `Integer` | `300` | The width/height of the image in pixels. |

**Success Response:**
* **Code:** 200 OK
* **Content:** `image/png`

## 🏗️ Project Structure

* **`QrCodeController.java`**: Handles the web requests and manages the image response headers.
* **`QrCodeService.java`**: Utilizes `QRCodeWriter` to encode the bit matrix and convert it into a PNG byte array.
* **`QrRequest.java`**: A Data Transfer Object (DTO) that holds the URL and size parameters.

## ⚙️ Setup Instructions

1. **Add Dependencies**:
   Ensure your `pom.xml` includes the ZXing libraries:
   ```xml
   <dependency>
       <groupId>com.google.zxing</groupId>
       <artifactId>core</artifactId>
       <version>3.5.3</version>
   </dependency>
   <dependency>
       <groupId>com.google.zxing</groupId>
       <artifactId>javase</artifactId>
       <version>3.5.3</version>
   </dependency>
