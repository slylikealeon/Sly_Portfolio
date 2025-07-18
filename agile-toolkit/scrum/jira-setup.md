# ⚙️ Jira Setup & Advanced Configuration

As a Scrum Master, Jira is one of my main tools to promote visibility, alignment, and delivery tracking across multiple teams and stakeholders. Beyond basic ticket tracking, I use Jira as a strategic layer to support planning, reduce blockers, and empower team autonomy.

---

## 🗂️ Project Structure & Issue Types

I configure Jira around clear, consistent structures to enable clarity and traceability.

### Standard Issue Types:
- **Epics:** Group features or workstreams into high-level deliverables
- **User Stories:** Functional requirements framed from the user’s perspective
- **Spikes:** Time-boxed investigation tasks to explore unknowns
- **Dependencies:** External or internal blockers that may impact delivery
- **Suggestions:** Future ideas or features outside the current scope
- **Bugs:** QA or production issues requiring attention

### Labels & Components:
I promote standardized use of **labels** and **components** to allow flexible filtering, reporting, and roadmap organization. These are also essential to visualize ownership, track domains (e.g., frontend, backend, infra), and segment work by module or product area.

---

## 🔍 Filters & Advanced JQL Usage

I regularly create and maintain **custom filters** using **Jira Query Language (JQL)** to drive dashboards, backlog views, and visibility boards. These filters help surface:

- Unresolved or aging issues
- Stories by epic, label, or component
- Sprint-level progress and exceptions
- Dependencies and blockers across squads

Additionally, I use plugins like **Speedrunner** to manage dynamic filters across boards, especially in scaled environments.

---

## 📊 Dashboards by Audience

Jira dashboards are tailored for different roles, ensuring each stakeholder sees the metrics they care about:

### For Development Teams:
- Sprint progress (by assignee, by epic)
- Blockers and flagged tickets
- Bugs opened/closed within the sprint

### For Product Owners:
- Readiness of backlog items
- Story points by priority and refinement status
- Capacity and team availability

### For Managers & Stakeholders:
- Epic-level burnup
- Delivery trends and velocity over time
- Dependency tracking and risk alerts

Dashboards include visual gadgets (e.g., pie charts, cumulative flow diagrams, filter statistics) and often combine both current sprint and trend data.

---

## 🧭 Roadmaps & Planning

I encourage the use of **Jira Roadmaps** to give long-term visibility and alignment. These include:

- Epics linked to features and initiatives
- Target delivery dates
- Swimlanes by product area or team
- Cross-epic dependency visualization

This roadmap setup supports sprint-level planning and higher-level PI (Program Increment) planning.

---

## 🛠️ Kanban Boards (Specialized)

Beyond Scrum boards, I configure **Kanban boards** to support teams with ongoing flow-based work, such as:

- Bug tracking and triage
- Support and maintenance queues
- DevOps or platform squads

These boards often include:
- Custom columns (e.g., “Waiting on PO”, “Staging Verified”)
- WIP limits to maintain flow
- Flags for blocked issues or SLA breaches
- Swimlanes by priority, type, or service area

---

## 🔄 Workflows & Automation

Workflows are adapted to each team’s context while maintaining consistency across squads.

- Typical flow: `To Do → In Progress → In Review → QA → Done`
- Custom statuses for blocked or escalated work
- Automation rules to:
  - Trigger status changes
  - Notify stakeholders
  - Auto-assign tickets based on labels or components
  - Link subtasks and parent tasks

---

## 🧠 Best Practices I Promote

- **Link stories to epics** and **subtasks to parent issues** for traceability
- Use **Definition of Ready/Done** checklists inside tickets
- Document conventions and standards in **Confluence**, linked from Jira
- Keep the backlog refined and clean — stories without value or clarity don’t make it into the sprint
- Promote **visual management** over excessive reporting

---

## 💡 Final Thought

I treat Jira as more than a tool—it's a reflection of how a team works and collaborates. My goal is to configure it in a way that’s intuitive, transparent, and actually helpful, giving every team member and stakeholder the clarity they need to make the right decisions.
