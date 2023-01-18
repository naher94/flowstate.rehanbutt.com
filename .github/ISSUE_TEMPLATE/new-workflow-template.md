---
name: New Workflow Template
about: New content issue template
title: ''
labels: add workflow
assignees: ''

---

- [ ] Record Workflow Experience
- [ ] Trim/Edit Recording
- [ ] Upload to YouTube
- [ ] Add to VideoAnt
- [ ] Add comments to VideoAnt
- [ ] Add to Flowstate site
  - [ ] Create a markdown file into the `_workflows` collection
  - [ ] Add the application, if new, to the ` _data/apps.yml`
    - [ ] Add application icon to `img/icons` (Template in Figma)
  - [ ] Add the application brand color as a variable to ` variables.scss`
  - [ ] Add the application specific `mini-card` to `design-system.scss`
    - `&.agenda{ @include mini-card($agenda-brand-color,$elevation); } `
  - [ ] Add the workflow type, if new, to the` _flow-types` collection
    - [ ] Add flow type icon to `img/flow-type` as `.svg` (Template in Figma)
- [ ] Increment site version in `config.yml` with each release
