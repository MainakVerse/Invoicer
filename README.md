# Parsing Invoices using Gemini 1.5 API with Google Apps Script

![](https://tanaikech.github.io/image-storage/20240403a/fig1.png)

# Abstract

This report explores using Gemini, a new AI model, to parse invoices in Gmail attachments. Traditional text searching proved unreliable due to invoice format variations. Gemini's capabilities can potentially overcome this inconsistency and improve invoice data extraction.

# Introduction

After Gemini, a large language model from Google AI, has been released, it has the potential to be used for modifying various situations, including information extraction from documents. In my specific case, I work with invoices in PDF format. Until now, I relied on the direct search by a Google Apps Script to achieve this task. The script's process involved:

1. Converting each invoice PDF file into a temporary Google Doc.
2. Utilizing text searching within the Google Doc to extract required values.
3. Deleting the temporary Google Doc after successful extraction.

However, this approach proved unreliable due to variations in the invoice formats of each invoice. The text-searching method often failed to capture the required values consistently across different invoice layouts. This inconsistency led me to believe that Gemini's capabilities could be a valuable asset for invoice parsing.

In this report, I aim to introduce a method for parsing various invoice types and retrieving the required values using Gemini. Here, I chose to leverage Google Apps Script for this project because the invoices are received as email attachments in Gmail. Google Apps Script provides a convenient way to access and process these PDF files directly within the Gmail environment.

