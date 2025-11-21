# README.md -- Wireshark Network Analysis Practical (ICT414)

This repository contains the submission for the
ICT414 -- Information
Security Final Practical.
The task involved capturing network traffic using Wireshark,
identifying an HTTP GET request to `www.rocktv.app`, analyzing the
packet details, and preparing a short report.

Repository contents: - `ict414_capture.pcapng` -- Wireshark packet
capture file

- `report_<Chanda David>.pdf` -- Analysis report.
- `README.md` -- Steps followed during the practical

---

## Steps Followed for Packet Capture and Analysis

### 1. Starting Wireshark

- Opened Wireshark on the computer.
- Selected the active network interface (Wi-Fi).
- Made sure the interface was receiving live packets.

---

### 2. Capturing Network Traffic

- Clicked Start Capture to begin recording.
- Allowed Wireshark to capture traffic for 1--2 minutes as
  instructed.

---

### 3. Generating the HTTP Traffic

- While capture was running, opened a browser.

- Visited the target website:

      www.rocktv.app

- This triggered the HTTP GET request required for analysis.

---

### 4. Filtering the Captured Packets

To isolate HTTP traffic, the following filters were used:

- HTTP packets only

      http

- Filter by local IP (optional for clarity)

      ip.addr == <your IP address>

Using these filters made it easier to locate the GET request and the
corresponding response.

---

### 5. Identifying the HTTP GET Request

From the filtered list: - Selected the HTTP GET request made to
`www.rocktv.app`. - Examined the detailed packet information under: -
Hypertext Transfer Protocol.

- Transmission Control Protocol.
- Internet Protocol

Extracted details included: - Client (source) IP address.

- Server (destination) IP address.
  www.rocktv.app
- HTTP response code.
- Interpretation of whether the request was successful

---

### 6. Capturing the Required Screenshot

- Took a clear screenshot showing the filtered HTTP packets (GET
  and response).

---

### 7. Saving the Capture File

- Saved the capture as required:

      ict414_capture.pcapng

---

### 8. Preparing the PDF Report

Created `report_<yourname>.pdf` containing: - Task description.

- Packet details and analysis.
- Screenshot of filtered HTTP traffic.
- Basic interpretation of the HTTP response.
- HTTP method.
- Timing differences

---

### 9. Uploading to GitHub

Final repository upload included: - `report_<yourname>.pdf` -
`ict414_capture.pcapng` - `README.md`

All files organized clearly as required.

---

## Conclusion

This practical demonstrated how to: - Capture network packets.

- Filter specific protocol traffic.
- Analyze HTTP requests and responses.
- Extract essential packet information.
- Document findings in a report.
