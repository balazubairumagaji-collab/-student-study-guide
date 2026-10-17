# Student Study Guide

An [Agent Skill](https://agentskills.io/specification) that helps students turn supplied course PDFs, notes, and other learning materials into clear summaries and study guides. It organizes ideas by topic, explains key terms using the source, can provide separate review questions and answers, and flags material that could not be read. It avoids unsupported guesses and does not do graded work for students.

## Folder structure

```text
student-study-guide/
├── SKILL.md   # Skill metadata and operating instructions
├── README.md  # Overview, installation, and validation
└── LICENSE    # MIT License, copyright 2026 Student Study Guide
```

There is no script: the skill's task is to read material available to its agent and respond with a source-grounded study aid.

## Installation

Install the `student-study-guide` folder in the skills directory recognized by your Agent Skills-compatible agent or host. The host's documentation determines that directory and whether it needs a reload or restart after installation. Keep the folder name `student-study-guide` so it matches the required `name` in `SKILL.md`.

To try the skill, provide course material and ask for a summary, study guide, or help reviewing the notes. The skill operates on material available in the conversation or through the host's file-reading capabilities; it does not independently extract or convert PDFs.

## Validation

From the directory containing this folder, run:

```sh
skills-ref validate ./student-study-guide
```

The validator checks Agent Skills metadata and naming conventions. It does not verify the accuracy of summaries produced for particular course materials.

## License

Distributed under the MIT License. See [LICENSE](LICENSE).
