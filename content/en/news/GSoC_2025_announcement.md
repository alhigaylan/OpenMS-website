# OpenMS Invites the Computational Mass Spectrometry Community to Join Google Summer of Code 2025! 

[Google Summer of Code (GSoC)](https://summerofcode.withgoogle.com) fantastic opportunity to contribute to the growth and innovation in the field of computational mass spectrometry by mentoring talented students from around the world. OpenMS is planning to apply as an umbrella organization and we would like to extend an invitation to other projects and groups within the computational mass spectrometry and proteomics/metabolomics communities to join us in this effort. If your project aligns with the goals of GSoC and you are interested in mentoring a student project, we encourage you to submit your proposals by Feburary 11th at 18:00 UTC 

As an umbrella organization, we would like to extend an invitation to other projects and groups within the computational mass spectrometry and proteomics/metabolomics communities to join us in this effort. If your project aligns with the goals of GSoC and you are interested in mentoring a student project, we encourage you to submit your proposals by **February 7th at 23:59 UTC.**

> **Note:** This webpage will be continuously updated to reflect new project proposals. Please check in regularly.

---

## Mentors

**GSoC is program** that connects open-source projects with enthusiastic contributors, fostering collaboration and the development of innovative solutions. By mentoring a GSoC project, you’ll have the opportunity to:

- Guide and inspire the next generation of developers and researchers.
- Gain valuable contributions to your project from highly motivated students.
- Strengthen the open-source community within computational mass spectrometry.

### Submitting a Proposal:

- Please read the [GSoC Mentor Guide](https://google.github.io/gsocguides/mentor/) to get a better idea of what it entails.  
- Mentors generally spend 3–5 hours per week mentoring their student.  
- OpenMS has an active [Discord server](https://discord.com/invite/4TAGhqJ7s5). This is the best way to contact the OpenMS team and coordinate project proposals and mentorship.  
- **The deadline to submit a project proposal as a mentor is February 11th at 18:00 UTC.**

---

## Students

- Make sure you are [eligible](https://summerofcode.withgoogle.com/get-started) to participate in GSoC 2025.  
- Read the [DOs and DON'Ts document](https://opensource.googleblog.com/2011/03/dos-and-donts-of-google-summer-of-code.html) to gauge your interest in participating in this year's GSoC.  
- Review the list of projects available below. If you have specific questions about a project, our mentors are active on [Discord](https://discord.com/invite/4TAGhqJ7s5) and will happily assist you.

---

## Projects

### 1) Integrate Apache Parquet into OpenMS Build System

**Proposed Mentors:** Timo Sachsenberg, Samuel Wein  
**Skills:** CMake, GitHub CI, C++, Python  
**Estimated Project Length:** 350 hours | **Difficulty:** Medium  

Proteomics and metabolomics mass spectrometry studies are generating datasets of unprecedented size as they scale to include more and more samples. Managing and processing these large datasets efficiently requires robust and scalable data handling solutions to make results readily available for downstream processing tasks like machine learning.

The task is to integrate Apache Parquet, a columnar storage format, into OpenMS as a fundamental step toward enabling faster data processing, reducing memory usage, and improving scalability. The integration will involve:

1. Updating the OpenMS build system with new CMake configurations.  
2. Developing comprehensive tests to validate functionality and performance.  
3. Adapting CI/CD pipelines for macOS, Linux, and Windows to ensure cross-platform compatibility.

---

### 2) Write a C++ library to read/write mzQC

**Proposed Mentors:** Chris Bielow,   
**Skills:**  C++, Controlled Vocabularies, JSON, CMake, GitHub CI  
**Estimated Project Length:** 350 hours | **Difficulty:** Easy to Medium

Adoption and public exposure of quality control in mass-spectrometry (MS) has gained increasing traction in recent years. The Proteomics Standard Initiative (PSI) has developed an open exchange format
named [mzQC](https://hupo-psi.github.io/mzQC/),which aims to foster capturing, exchanging and archiving quality control related data across all MS-based OMICS, such as proteomics, metabolomics and lipidomics.
Currently, there exist core libraries to read and write mzQC in Python, R, and Java. See [MS-Quality-Hub](https://github.com/MS-Quality-Hub).  

Tasks:

1. implement a new mzQC Core library in C++ which supports reading/writing of mzQC
2. publish the library on GitHub under a permissive license (BSD-3clause) as a subproject of [MS-Quality-Hub](https://github.com/MS-Quality-Hub).
3. write class/unit tests and run them using GithubActions
4. integrate your library into OpenMS (incl. adaptation of the build system to include your library) and substitute existing code to create an mzQC

---

### 3) Write a generic visualization app for mzQC

**Proposed Mentors:** Chris Bielow, Arslan Siraj   
**Skills:**  Visualization, Controlled Vocabularies, Python|R  
**Estimated Project Length:** 175 hours | **Difficulty:** Easy to Medium

Adoption and public exposure of quality control in mass-spectrometry (MS) has gained increasing traction in recent years. The Proteomics Standard Initiative (PSI) has developed an open exchange format
named [mzQC](https://hupo-psi.github.io/mzQC/), which aims to foster capturing, exchanging and archiving quality control related data across all MS-based OMICS, such as proteomics, metabolomics and lipidomics.
Currently, there exists no package which is capable of visualizing and summarizing the content of any given mzQC file (e.g. as obtained from a publication's supplemental material). 

Tasks:

1.  Pick a visualization framework of your choice (e.g. Streamlit or R Shiny) and write code (Python or R) to allow a user to explore the content of a given (uploaded) mzQC file.
2. Visualization could be a textual summary as well as (interactive) plots for the QC data contained within the mzQC file. Depending on the metrics properties, automated plot types should be chosen.

---

**Let’s make GSoC 2025 a memorable and productive experience for everyone involved!**

Best regards,  
The OpenMS-Developers
