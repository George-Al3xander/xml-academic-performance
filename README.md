# Academic Performance XML

This repository contains an XML document that represents academic performance details for students enrolled in a Bachelor of Science in Computer Science program. The XML structure includes subjects, majors, groups, students, and their exam results.

## XML Structure

The XML file follows a hierarchical structure:

- `<performance>`: Root element containing all academic data.
  - `<subject>`: Represents a course.
    - `<code>`: Course identifier.
    - `<title>`: Course name.
    - `<cycle>`: Course category (e.g., core).
    - `<reporting>`: Status of grade reporting.
    - `<major>`: Represents the academic program.
      - `<code>`: Major identifier.
      - `<title>`: Name of the academic program.
      - `<group>`: Represents a student group.
        - `<number>`: Group number.
        - `<name>`: Group name.
        - `<student>`: Represents an individual student.
          - `<name>`: Student's full name.
          - `<code>`: Student's unique code.
          - `<id>`: Student's unique identifier.
          - `<exam>`: Represents an exam attempt.
            - `<date>`: Exam date.
            - `<grade>`: Score received.

## Example XML

```xml
<performance>
    <subject>
        <code>CS101</code>
        <title>Object-oriented programming</title>
        <cycle>core</cycle>
        <reporting>ongoing</reporting>
        <major>
            <code>122</code>
            <title>Bachelor of Science in Computer Science</title>
            <group>
                <number>23</number>
                <name>CS</name>
                <student>
                    <name>Al Pacino</name>
                    <code>143</code>
                    <id>4882</id>
                    <exam>
                        <date>12.04.2024</date>
                        <grade>88</grade>
                    </exam>
                </student>
            </group>
        </major>
    </subject>
</performance>
```

## Usage

This XML structure can be used for:

- Academic performance tracking.
- Data integration with student management systems.
- Generating reports or visualizations.

## How to Use

1. Clone the repository:
   ```sh
   git clone https://github.com/George-Al3xander/xml-academic-performance
   ```
2. Open the XML file with any text editor or XML viewer.
3. Use XSLT or CSS for styling and transformation if needed.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

