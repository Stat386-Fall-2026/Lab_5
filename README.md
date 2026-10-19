# Lab 5: Regex, Cleaning, Joins, and Pipelines

## Objective

Use regular expressions to clean and standardize General Conference talk data, join datasets, and build data-processing pipelines. You will extract and transform text, handle inconsistencies and missing values, combine information across datasets, and explore patterns in talk content.

## Create your personal repository

1. Click **Use this template** and select **Create a new repository**.
2. For **Owner**, select `Stat386-Fall-2026`.
3. Name your repository using the format `your_netid_lab_5`.
4. Set the repository visibility to **Private**.
5. Click **Create repository**.

## Clone and set up the project

Clone your personal repository inside your `School/STAT_386` folder:

```bash
git clone <your-repository-url>
cd <your-repository-name>
```

Install the project dependencies:

```bash
uv sync
```

The first time you run this command, `uv` will create a `uv.lock` file. Include
that file in your first commit.

Open the repository folder in Positron. If Positron asks you to select a Python
interpreter, select the interpreter inside the `.venv` folder created by `uv`.

## Complete the lab

Open `lab_5.qmd` and replace `Your Name` with your name. Complete every code
section and every written response. You can preview the document while you
work by running:

```bash
uv run quarto preview lab_5.qmd
```

Stop the preview by pressing `Ctrl+C` in the terminal.

Make several meaningful commits as you work. For example:

```bash
git add lab_5.qmd
git commit -m "Create keyword features"
git push
```

## Render and submit

Before submitting, restart your work from a clean session and render the final
document:

```bash
uv run quarto render lab_5.qmd
```

Commit and push both the source document and the rendered HTML file:

```bash
git add lab_5.qmd lab_5.html uv.lock
git commit -m "Complete Lab 4"
git push
```

Follow the submission directions provided in Canvas.

## Work with the AI Collaborator

During this lab, you will interact with the course AI collaborator twice. Each interaction will create a Pull Request containing a proposed change to your repository.

For each Pull Request, carefully review both the proposed code and the questions included in the Pull Request description. Do not assume that a proposed change should automatically be accepted.

### First AI Collaborator Interaction

Create a new Issue using the **Lab 5 Complete** Issue template if it is available.

Use the following title:

```text
Lab 5 complete
```

The Issue description can be empty.

Post the first AI collaborator processing command as a new comment on the Issue:

```text
@local-llm-user process config-dir: Lab_5/metadata_01.yml in instructor-repo: Stat386-Fall-2026/Instructor_Repo
```

The command must be posted as a comment, not in the Issue description.

Once the collaborator finishes processing your repository, it will create a Pull Request.

1. Open the Pull Request created by the collaborator.
2. Read the Pull Request description carefully.
3. Review the proposed changes in the **Files changed** tab.
4. Answer each question included in the Pull Request description.
5. Post your answers as a comment on that Pull Request.
6. Decide whether the proposed change should be included in your repository based on your review.

If you merge the Pull Request, update your local repository before continuing:

```bash
git pull
```

Make sure you understand the changes that were added before continuing with the lab.

### Second AI Collaborator Interaction

After completing your review of the first Pull Request, return to the same Lab 5 completion Issue.

Post the second AI collaborator processing command as a new comment:

```text
@local-llm-user process config-dir: Lab_5/metadata_02.yml in instructor-repo: Stat386-Fall-2026/Instructor_Repo
```

Once processing is complete, the collaborator will create a second Pull Request.

1. Open the second Pull Request.
2. Read the Pull Request description carefully.
3. Review the proposed changes in the **Files changed** tab.
4. Answer each question included in the Pull Request description.
5. Post your answers as a comment on that Pull Request.
6. Decide whether the proposed change should be included in your repository based on your review.

Remember that code can run successfully without necessarily being an appropriate change to the analysis. Your goal is to evaluate the proposed change rather than automatically accept it.

If you merge the second Pull Request, update your local repository again:

```bash
git pull
```

Complete both AI collaborator interactions and respond to the questions in both Pull Requests before finishing the lab.

## Before you finish

- [ ] Your name appears in the document header.
- [ ] Every code section is complete.
- [ ] Every written response is complete.
- [ ] Your term counts are case-insensitive.
- [ ] You compare raw counts with rates based on talk length.
- [ ] Every plot has a useful title and axis labels.
- [ ] `lab_5.qmd` renders without errors.
- [ ] `lab_5.html` and `uv.lock` are committed.
- [ ] All commits are pushed to GitHub.
- [ ] You answered the collaborator's questions.


## Repository contents
```text
Lab_5/
├── data/
│   ├── raw/
│   │   ├── talks_raw.csv
│   │   └── speaker_metadata_raw.csv
│   └── processed/
│       └── talks_clean.csv
├── .github/
│   └── ISSUE_TEMPLATE/
│       └── lab-5-complete.md
├── .gitignore
├── README.md
├── lab_5.qmd
├── pyproject.toml
└── uv.lock
```
