

# EXP 5: Comparing Prompting Techniques Through Engineering Problem-Solving Scenarios

# Aim:To compare different prompting techniques and evaluate their effectiveness in solving real-world engineering problems by using a problem selected from a student's 3rd-year or final-year project work. 

### AI Tools Required: 

# EXPERIMENT OVERVIEW

In this experiment, each student/team selects a genuine problem from their ongoing or completed 3rd-year or final-year engineering project.
The same engineering problem is given to an AI system using different prompting techniques. Students then compare the responses based on relevance, accuracy, completeness, clarity, feasibility and usefulness.
The purpose is not simply to obtain an AI-generated answer. Students must analyse how changing the prompting technique changes the quality of the solution.

EXPERIMENT PROCEDURE
Step 1 – Select the Engineering Problem
Choose one genuine problem from the student's 3rd-year or final-year project.
Step 2 – Write the Base Prompt
Write a simple prompt describing the engineering problem without using advanced prompting techniques.
Step 3 – Apply Different Prompting Techniques
Rewrite the same problem using at least four different prompting techniques.
For example:
Technique 1 – Straightforward Prompt
Suggest a method to detect crop diseases using computer vision.structure.
Run Experiments with ChatGPT:
Input the naïve prompt for each scenario and record the generated response.
Then input the corresponding basic prompt and capture that response.
Repeat this process for all selected scenarios to gather a full set of results.
Evaluate Responses : 
	Compare how ChatGPT performs when given naïve versus basic prompts and analyze the output based on Quality,Accuracy and Depth. Also analyse does ChatGPT consistently provide better results with basic prompts? Are there scenarios where naïve prompts work equally well?
Deliverables:
A table comparing ChatGPT's responses to naïve and basic prompts across all scenarios.
Analysis of how prompt clarity impacts the quality, accuracy, and depth of ChatGPT’s outputs.
Summary of findings with insights on how to structure prompts for optimal results when using ChatGPT.

#**STUDENT SUBMISSION FORMAT**
Each student/team should submit:
Project title and problem statement
Selected engineering scenario
Base prompt
Minimum four improved prompts using different techniques
AI-generated outputs
Comparison/evaluation table
Analysis and observations
Final selected prompting technique
Refined/final prompt
Engineering validation

**Conclusion**

# OUTPUT
```
# EXPERIMENT NO: 5

# COMPARING PROMPTING TECHNIQUES THROUGH ENGINEERING PROBLEM-SOLVING SCENARIOS

---

## 1. AIM

To compare different prompting techniques and evaluate their effectiveness in solving real-world engineering problems using Generative AI (ChatGPT). The experiment aims to understand how prompt structure, clarity, context and constraints influence the relevance, accuracy, completeness, clarity, feasibility and usefulness of AI-generated solutions.

## 2. AI TOOLS REQUIRED

| S. No. | Tool | Purpose |
|---|---|---|
| 1 | ChatGPT | Generating and comparing AI responses |
| 2 | Python | Backend programming |
| 3 | OpenCV | Image processing |
| 4 | YOLO | Vehicle and number plate detection |
| 5 | EasyOCR | Number plate text recognition |
| 6 | FastAPI | Backend API development |
| 7 | React | User interface development |
| 8 | SQLite | Vehicle information storage |

## 3. PROJECT TITLE

**SMARTROAD AI – Intelligent Vehicle Identity and Traffic Safety System**

## 4. PROBLEM STATEMENT

Traditional traffic monitoring systems mainly depend on manual vehicle verification and basic number plate recognition. These methods may fail to identify stolen vehicles, cloned number plates and unauthorized vehicles effectively.

Identifying suspicious vehicles manually requires considerable time and effort. There is also a possibility of human errors during vehicle verification.

To overcome these challenges, SMARTROAD AI is proposed as an AI-based vehicle identification and traffic safety system.

The system uses cameras, computer vision and Optical Character Recognition (OCR) to identify vehicle registration numbers. The extracted information is compared with registered vehicle records stored in a database.

The system generates alerts when stolen vehicles, unknown registrations or suspicious vehicle information mismatches are detected. It provides a dashboard for traffic police and administrators to monitor vehicle activities.

## 5. SELECTED ENGINEERING SCENARIO

The selected engineering scenario is the development of an intelligent vehicle identification and traffic monitoring system using Artificial Intelligence.

### 5.1 Main Objectives

1. To automatically detect vehicle number plates using camera images.
2. To recognize registration numbers using OCR technology.
3. To retrieve registered vehicle information from a database.
4. To identify stolen vehicles using stored records.
5. To detect possible cloned number plates through suspicious mismatches.
6. To generate alerts for traffic authorities.
7. To provide a user-friendly monitoring dashboard.

### 5.2 Proposed System Architecture

The following diagram represents the overall architecture of SMARTROAD AI.

```text
          VEHICLE MOVING ON ROAD
                    |
                    v
             CCTV / CAMERA
                    |
                    v
          IMAGE CAPTURE MODULE
                    |
                    v
        VEHICLE AND PLATE DETECTION
                (YOLO)
                    |
                    v
          NUMBER PLATE IMAGE
                    |
                    v
            OCR PROCESSING
              (EasyOCR)
                    |
                    v
        REGISTRATION NUMBER
                    |
                    v
          BACKEND PROCESSING
               (FastAPI)
                    |
                    v
           VEHICLE DATABASE
                (SQLite)
                    |
                    v
           VERIFICATION MODULE
                    |
          +---------+---------+
          |         |         |
          v         v         v
       VERIFIED   STOLEN   SUSPICIOUS
       VEHICLE    VEHICLE   MISMATCH
          |         |         |
          v         v         v
        DISPLAY    ALERT     ALERT
          +---------+---------+
                    |
                    v
           ADMIN DASHBOARD
                 (React)
                    |
                    v
            TRAFFIC AUTHORITIES
```

**Figure 1: Overall Architecture of SMARTROAD AI**

### 5.3 Working Principle

The system works through the following stages:

- **Image Capture:** A camera captures the vehicle image at a traffic junction.
- **Vehicle Detection:** YOLO detects the vehicle and identifies the number plate region.
- **Text Recognition:** EasyOCR extracts the registration number from the number plate.
- **Database Search:** The backend retrieves the corresponding registered vehicle details.
- **Verification:** The system checks the vehicle's registration and available records.
- **Alert Generation:** Stolen vehicles and suspicious mismatches generate alerts.
- **Dashboard Display:** The results are displayed to traffic authorities.

Note: Chassis and engine numbers are maintained as registered database information. The prototype does not attempt to scan these identifiers from moving vehicles.

## 6. BASE PROMPT (NAÏVE PROMPT)

A naïve prompt is a simple instruction given to an AI system without providing detailed context, specific requirements or output constraints.

**Prompt:**

"Develop an AI-based vehicle identification system for traffic safety."

### AI-Generated Output

An AI-based vehicle identification system can use cameras and machine learning techniques to detect vehicles and recognize their number plates.

Optical Character Recognition (OCR) can extract registration numbers from images. These numbers can be compared with a vehicle database to identify registered and suspicious vehicles.

The system can also generate alerts for stolen vehicles and help traffic authorities monitor road safety.

### Evaluation

The response provides a basic understanding of the proposed system. However, it does not explain the system architecture, implementation technologies, database structure or detailed working procedure.

## 7. IMPROVED PROMPTS USING DIFFERENT PROMPTING TECHNIQUES

Four improved prompting techniques are applied to the same engineering problem to understand their effectiveness.

### TECHNIQUE 1 – ROLE-BASED PROMPTING

**Definition:**

Role-based prompting assigns a specific role or professional identity to the AI system. It helps generate responses from the perspective of a particular expert.

**Prompt:**

"Act as an experienced Artificial Intelligence and Machine Learning engineer. Design an intelligent vehicle identification system called SMARTROAD AI using Automatic Number Plate Recognition (ANPR).

Explain how cameras, computer vision, OCR and machine learning can be used to detect number plates, retrieve vehicle details and identify stolen or suspicious vehicles.

Provide a suitable technical architecture, important modules, implementation technologies and development steps."

**AI-Generated Output:**

SMARTROAD AI can be developed using a camera-based vehicle detection system and an OCR-based number plate recognition module.

**1. Vehicle Detection Module**

Cameras capture images of vehicles passing through traffic junctions. Computer vision techniques identify vehicles in the captured images.

**2. Number Plate Detection Module**

YOLO can be used to locate number plates within vehicle images.

**3. OCR Processing Module**

EasyOCR extracts the registration number from the detected number plate.

**4. Database Verification Module**

The extracted registration number is compared with the vehicle information stored in the database.

**5. Alert Generation Module**

The system identifies stolen vehicles and suspicious registration details and generates alerts.

**6. Dashboard Module**

A web dashboard displays vehicle details, detection history and alerts for traffic authorities.

**Suggested Technologies:**

| Component | Technology |
|---|---|
| Programming | Python |
| Image Processing | OpenCV |
| Object Detection | YOLO |
| Text Recognition | EasyOCR |
| Backend | FastAPI |
| Frontend | React |
| Database | SQLite |

**Evaluation:**

Role-based prompting produces a professional and technically organized response. It identifies the major modules and suggests technologies suitable for the project.

---

### TECHNIQUE 2 – CONTEXT-BASED PROMPTING

**Definition:**

Context-based prompting provides background information about the problem before asking the AI system to generate a solution. It helps the AI understand the actual situation and requirements.

**Prompt:**

"In many cities, traffic authorities face difficulties identifying stolen vehicles and detecting cloned number plates. Manual verification takes time and may lead to errors.

Design a SMARTROAD AI system that captures vehicle number plates at traffic junctions, retrieves registered vehicle details and checks them against a vehicle database.

The system should identify stolen vehicles, detect possible cloned number plates through suspicious mismatches and notify traffic police.

Explain the complete workflow, technologies, challenges and possible solutions."

**AI-Generated Output:**

SMARTROAD AI can provide an automated vehicle verification process to improve traffic monitoring.

**1. Problem Identification**

Manual vehicle verification is time-consuming and may not identify suspicious vehicles quickly.

**2. Camera-Based Monitoring**

CCTV cameras capture vehicle images at selected traffic junctions.

**3. Number Plate Recognition**

Computer vision identifies the number plate, and OCR extracts its registration number.

**4. Vehicle Database Verification**

The extracted registration number is checked against registered vehicle information.

**5. Suspicious Vehicle Identification**

The system checks whether the vehicle is reported stolen or whether available vehicle information indicates a possible mismatch.

**6. Alert Notification**

Suspicious vehicles are reported through the monitoring dashboard.

**7. Possible Challenges and Solutions**

| Challenge | Possible Solution |
|---|---|
| Poor lighting | Image enhancement |
| Blurred images | Image preprocessing |
| OCR errors | Confidence-based verification |
| Network failure | Local data storage |
| Incorrect records | Database validation |
| False alerts | Human verification |

**Evaluation:**

Context-based prompting provides a solution that is closely connected to the real-world traffic problem. It also identifies practical challenges and possible solutions.

---

### TECHNIQUE 3 – STEP-BY-STEP PROMPTING

**Definition:**

Step-by-step prompting divides a complex problem into smaller and manageable tasks. It encourages the AI system to provide an organized solution in a logical sequence.

**Prompt:**

"Design SMARTROAD AI by following these steps:

1. Explain the vehicle detection process.
2. Describe number plate localization and recognition.
3. Explain OCR-based registration number extraction.
4. Describe vehicle database verification.
5. Explain stolen vehicle and possible cloned plate detection.
6. Describe alert generation and dashboard implementation.
7. Suggest suitable technologies and testing methods.

Present the solution in a structured engineering format."

**AI-Generated Output:**

The SMARTROAD AI system can be implemented through the following stages.

**Step 1: Vehicle Detection**

Use CCTV cameras to capture vehicle images at traffic junctions.

**Step 2: Number Plate Localization**

Apply computer vision models such as YOLO to locate the number plate region.

**Step 3: Number Plate Recognition**

Use OCR technology to extract the registration number from the detected plate.

**Step 4: Database Verification**

Compare the extracted registration number with registered vehicle information stored in the database.

**Step 5: Suspicious Vehicle Detection**

Check stolen vehicle records and identify possible cloned number plates through suspicious registration or vehicle information mismatches.

**Step 6: Alert Generation**

Generate notifications when a stolen vehicle or suspicious mismatch is detected.

**Step 7: Dashboard Development**

Develop a web dashboard to display vehicle details, detection history and alerts.

**Step 8: System Testing**

Test the system using different vehicle images, lighting conditions and sample database records.

**Implementation Workflow:**

```text
START
  |
  v
Capture Vehicle Image
  |
  v
Detect Number Plate
  |
  v
Extract Registration Number
  |
  v
Search Vehicle Database
  |
  v
Verify Vehicle Information
  |
  v
Is Vehicle Suspicious?
  |
  +------ YES ------> Generate Alert
  |                         |
  |                         v
  |                    Notify Authority
  |
  +------ NO -------> Display Verified Details
                            |
                            v
                           END
```

**Figure 2: Step-by-Step Working Flowchart**

**Evaluation:**

Step-by-step prompting provides a clear and systematic explanation of the entire system. It makes the implementation process easier to understand and follow.

---

### TECHNIQUE 4 – CONSTRAINT-BASED PROMPTING

**Definition:**

Constraint-based prompting specifies the conditions, limitations, requirements and technologies that the AI system must follow while generating a solution.

**Prompt:**

"Develop a practical SMARTROAD AI vehicle identification system with the following constraints:

1. Use number plate recognition through camera images.
2. Use OCR for registration number extraction.
3. Store vehicle information in a database.
4. Identify stolen vehicles and suspicious number plate mismatches.
5. Do not depend on scanning moving vehicles' chassis or engine numbers.
6. Generate alerts for traffic authorities.
7. Use affordable and open-source technologies.
8. Provide a solution suitable for a student engineering project prototype.

Explain the architecture, modules, implementation process and limitations."

**AI-Generated Output:**

SMARTROAD AI can be implemented as an affordable prototype using open-source technologies.

**Main Modules:**

| Module | Function |
|---|---|
| Camera Input | Captures vehicle number plate images |
| Image Processing | Enhances images and detects number plates |
| OCR Processing | Extracts registration numbers |
| Vehicle Database | Stores vehicle registration and associated details |
| Verification | Checks stolen vehicle records and suspicious mismatches |
| Alert System | Notifies authorities about suspicious vehicles |
| Admin Dashboard | Displays vehicle information and alerts |

**System Implementation:**

- Python is used for the main application logic.
- OpenCV processes captured images.
- YOLO detects number plates.
- EasyOCR extracts registration numbers.
- FastAPI connects the frontend and backend.
- SQLite stores vehicle information.
- React provides the monitoring dashboard.

**Important Limitations:**

- Poor-quality images may affect recognition.
- Incorrect database records may generate false alerts.
- Cloned plate detection requires additional evidence.
- Human verification is necessary before taking enforcement action.
- The prototype must use authorized vehicle data.

**Evaluation:**

Constraint-based prompting produces a practical and feasible solution. It follows the project requirements, avoids unnecessary features and considers implementation limitations.

## 8. COMPARISON OF NAÏVE AND IMPROVED PROMPTS

The following table compares the responses generated using different prompting techniques.

| Evaluation Criteria | Naïve | Role-Based | Context-Based | Step-by-Step | Constraint-Based |
|---|---|---|---|---|---|
| Relevance | Medium | High | Very High | High | Very High |
| Accuracy | General | High | High | High | High |
| Completeness | Low | High | High | Very High | Very High |
| Clarity | Medium | High | High | Very High | Very High |
| Feasibility | Low | High | High | High | Very High |
| Usefulness | Medium | High | Very High | Very High | Very High |

**Table 1: Qualitative Comparison of Prompting Techniques**

## 9. RESPONSE EVALUATION TABLE

The responses are evaluated using a five-point scale.

| Score | Meaning |
|---|---|
| 1 | Poor |
| 2 | Below Average |
| 3 | Average |
| 4 | Good |
| 5 | Excellent |

### 9.1 Evaluation Scores

| Prompting Technique | Relevance | Accuracy | Completeness | Clarity | Feasibility | Total |
|---|---:|---:|---:|---:|---:|---:|
| Naïve | 3 | 3 | 2 | 3 | 2 | 13/25 |
| Role-Based | 4 | 4 | 4 | 4 | 4 | 20/25 |
| Context-Based | 5 | 4 | 4 | 4 | 4 | 21/25 |
| Step-by-Step | 4 | 4 | 5 | 5 | 4 | 22/25 |
| Constraint-Based | 5 | 4 | 5 | 5 | 5 | 24/25 |

**Table 2: Prompt Evaluation Scores**

Note: These are illustrative evaluation scores based on the sample responses, not measured experimental accuracy.

### 9.2 Comparison of Prompt Structures

| Technique | Main Focus | Major Advantage |
|---|---|---|
| Naïve | Simple instruction | Quick response |
| Role-Based | Assigning an expert role | Professional output |
| Context-Based | Providing background | Problem-specific response |
| Step-by-Step | Dividing tasks | Organized explanation |
| Constraint-Based | Defining requirements | Practical solution |

## 10. ANALYSIS AND OBSERVATIONS

The experiment demonstrates that prompting techniques significantly influence the quality of AI-generated responses.

### 10.1 Analysis

**1. Naïve Prompting**

The naïve prompt produces a general solution. It is useful for obtaining basic information but lacks detailed implementation guidance.

**2. Role-Based Prompting**

Role-based prompting improves the technical quality of the response by assigning an expert role to the AI system.

**3. Context-Based Prompting**

Context-based prompting helps the AI understand the real-world problem and provides relevant solutions based on the given situation.

**4. Step-by-Step Prompting**

Step-by-step prompting organizes complex engineering problems into smaller tasks. It improves clarity and completeness.

**5. Constraint-Based Prompting**

Constraint-based prompting generates practical solutions by considering technical requirements, project limitations and available resources.

### 10.2 Major Observations

1. Clear prompts generate more relevant responses than vague prompts.
2. Providing background information improves problem understanding.
3. Assigning roles improves the professional structure of responses.
4. Dividing complex tasks improves the organization of technical solutions.
5. Specifying constraints makes generated solutions more practical.
6. Improved prompts reduce ambiguity and unnecessary information.
7. AI-generated solutions still require human verification and engineering testing.

### 10.3 Analysis of Prompt Effectiveness

The illustrative evaluation scores show that constraint-based prompting achieves the highest overall score, followed by step-by-step prompting.

This is because constraint-based prompting considers the actual requirements of the engineering project and produces a solution that is more suitable for implementation.

However, different techniques may be more useful for different engineering tasks. Combining techniques can also improve the overall quality of a prompt.

## 11. FINAL SELECTED PROMPTING TECHNIQUE

**Selected Technique: CONSTRAINT-BASED PROMPTING**

Constraint-based prompting is selected as the most suitable technique for the SMARTROAD AI engineering project.

### Reasons for Selection

- Defines clear project requirements.
- Considers available technologies and resources.
- Avoids unnecessary system features.
- Provides practical implementation guidance.
- Identifies technical limitations.
- Improves the feasibility of the proposed solution.

## 12. REFINED / FINAL PROMPT

The following prompt combines role-based, context-based, step-by-step and constraint-based prompting to generate a comprehensive engineering solution.

**Final Prompt:**

"Act as a professional Artificial Intelligence and Software Engineer. Develop a complete SMARTROAD AI vehicle identification and traffic safety system using Automatic Number Plate Recognition (ANPR).

The system must capture vehicle number plates using traffic cameras, detect the plate using computer vision, extract registration numbers using OCR and retrieve registered vehicle information from a database.

It must identify stolen vehicles, detect possible cloned number plates through suspicious mismatches and generate alerts when suspicious vehicle information is found.

Follow these constraints:

1. Use Python, OpenCV and YOLO for image processing and detection.
2. Use EasyOCR for number plate text extraction.
3. Use FastAPI for backend development.
4. Use React for the frontend dashboard.
5. Use SQLite for storing vehicle records.
6. Do not attempt to scan chassis or engine numbers from moving vehicles; use registered database information for verification.
7. Include suitable security and data validation measures.
8. Explain the system architecture, modules, workflow, database design, implementation steps and testing methods.
9. Identify possible limitations and suggest improvements.
10. Provide a realistic and cost-effective solution suitable for an engineering student project prototype.

Present the answer in a clear, structured and detailed engineering format."

## 13. ENGINEERING VALIDATION

Engineering validation is performed to determine whether the proposed system meets its functional requirements.

### 13.1 Test Cases

| Test Case | Input | Expected Result |
|---|---|---|
| TC01 | Clear number plate image | Correct registration number recognition |
| TC02 | Blurred number plate image | Low-confidence detection or manual verification |
| TC03 | Registered vehicle | Vehicle details retrieved successfully |
| TC04 | Stolen vehicle record | Stolen vehicle alert generated |
| TC05 | Unknown registration number | Unregistered vehicle notification |
| TC06 | Possible cloned number plate | Suspicious mismatch alert generated |
| TC07 | Database unavailable | Error notification displayed |
| TC08 | Poor lighting conditions | Image enhancement or manual verification |

**Table 3: Engineering Test Cases**

### 13.2 Validation Methods

**1. Recognition Testing**

Test the OCR module using clear, blurred and differently illuminated number plate images.

**2. Database Testing**

Verify whether the extracted registration number retrieves the correct vehicle information.

**3. Stolen Vehicle Testing**

Use sample stolen vehicle records to verify whether the system generates the expected alerts.

**4. Mismatch Testing**

Compare available vehicle information with registered records to identify suspicious inconsistencies.

**5. Performance Testing**

Measure processing time, OCR recognition accuracy and alert generation time using a defined test dataset.

**6. User Interface Testing**

Verify whether the dashboard correctly displays vehicle information and suspicious vehicle alerts.

### 13.3 Expected Validation Outcome

The prototype is expected to recognize clear number plates, retrieve matching vehicle information and generate alerts for predefined suspicious test cases.

Actual performance must be established through execution and measured test results.

## 14. ADVANTAGES OF THE PROPOSED SYSTEM

1. Reduces manual vehicle verification efforts.
2. Provides faster number plate identification.
3. Helps authorities identify vehicles reported stolen.
4. Supports detection of possible cloned number plates.
5. Provides centralized vehicle information.
6. Improves traffic monitoring efficiency.
7. Uses affordable and open-source technologies.
8. Provides a scalable foundation for future development.

## 15. FUTURE ENHANCEMENTS

1. Integrate real-time CCTV camera feeds.
2. Improve OCR performance under different lighting conditions.
3. Introduce advanced vehicle classification models.
4. Develop mobile notifications for authorized traffic personnel.
5. Integrate with authorized vehicle registration and stolen vehicle databases.
6. Improve cloned plate detection using additional visual evidence.
7. Introduce cloud-based monitoring and reporting.

## 16. CONCLUSION

Thus, different prompting techniques were successfully applied to the SMARTROAD AI engineering problem using ChatGPT. The generated responses were compared based on relevance, accuracy, completeness, clarity, feasibility and usefulness.

The experiment demonstrated that improved prompting techniques produce more structured, detailed and practical solutions than simple naïve prompts. Role-based prompting provided professional technical guidance, context-based prompting improved problem understanding, and step-by-step prompting organized the implementation process.

Constraint-based prompting was selected as the most suitable technique because it considers project requirements, technical limitations and implementation feasibility. Combining multiple prompting techniques further helped develop a refined prompt for obtaining a comprehensive engineering solution.

## 17. RESULT

**RESULT:** The experiment was successfully executed using different prompting techniques in ChatGPT. The AI-generated responses were compared and evaluated, and constraint-based prompting was selected as the most suitable technique for solving the SMARTROAD AI engineering problem.


# RESULT: The prompt for the above said problem executed successfully
