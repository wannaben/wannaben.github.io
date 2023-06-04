---
layout: default-layout
title: v9.6.20 User Guide - Dynamsoft Barcode Reader JavaScript Edition
description: This is the user guide of Dynamsoft Barcode Reader JavaScript SDK.
keywords: user guide, javascript, js
breadcrumbText: User Guide
noTitleIndex: true
needGenerateH3Content: true
needAutoGenerateSidebar: true
permalink: /programming/javascript/user-guide/index.html
---

<!--The original doc is hosted here => https://github.com/dynamsoft-docs/barcode-reader-docs-js/blob/preview/programming/javascript/user-guide/index.md -->

# Barcode Reader for Your Website - User Guide

[Dynamsoft Barcode Reader JavaScript Edition](https://www.dynamsoft.com/barcode-reader/sdk-javascript/) (DBR-JS) is equipped with industry-leading algorithms for exceptional speed, accuracy and read rates in barcode reading. Using its well-designed API, you can turn your web page into a barcode scanner with just a few lines of code.

![version](https://img.shields.io/npm/v/dynamsoft-javascript-barcode.svg)
![downloads](https://img.shields.io/npm/dm/dynamsoft-javascript-barcode.svg)
![jsdelivr](https://img.shields.io/jsdelivr/npm/hm/dynamsoft-javascript-barcode.svg)
![vulnerabilities](https://img.shields.io/snyk/vulnerabilities/npm/dynamsoft-javascript-barcode.svg)

Once the DBR-JS SDK gets integrated into your web page, your users can access a camera via the browser and read barcodes directly from its video input.

<video id="myVideo" controls width="400" autoplay="true">
    <source src="https://tst.dynamsoft.com/public/docs/dbr/javascript/How%20to%20Use%20Dynamsoft%20Barcode%20Reader%20JavaScript%20SDK%20v1.1.mp4">
</video>

<script>
    // Check if autoplay flag exists in sessionStorage
    const autoplayFlag = sessionStorage.getItem('autoplay');

    if (!autoplayFlag) {
        // Autoplay the video if the flag doesn't exist
        const videoElement = document.getElementById('myVideo');
        videoElement.autoplay = true;

        // Set the autoplay flag in sessionStorage
        sessionStorage.setItem('autoplay', 'true');
    } else {
        // Video autoplay is disabled for subsequent visits
        const videoElement = document.getElementById('myVideo');
        videoElement.autoplay = false;
    }
</script>

In this guide, you will learn step by step on how to integrate the DBR-JS SDK into your website.

<span style="font-size:20px">Table of Contents</span>

- [Hello World - Simplest Implementation](#hello-world---simplest-implementation)
  - [Understand the code](#understand-the-code)
  - [Run the example](#run-the-example)
- [Building your own page](#building-your-own-page)
  - [Include the SDK](#include-the-sdk)
  - [Configure the SDK](#configure-the-sdk)
  - [Interact with the SDK](#interact-with-the-sdk)
  - [Customize the UI (optional)](#customize-the-ui-optional)
- [API Documentation](#api-documentation)
- [System Requirements](#system-requirements)
- [How to Upgrade](#how-to-upgrade)
- [Release Notes](#release-notes)
- [Next Steps](#next-steps)

- [About](about.md)
- [Contact](contact.md)


