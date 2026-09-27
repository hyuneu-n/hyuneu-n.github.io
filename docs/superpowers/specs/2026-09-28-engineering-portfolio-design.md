# Hyuneun Seo Engineering Portfolio Design

## Goal

Turn the Academic Pages repository into a fast, engineering-focused portfolio for global technical roles including Config Intelligence AI Solutions Engineer, Google Camera System Software, and Furiosa AX Engineer.

## Audience and positioning

The site should help an engineering recruiter quickly understand that Hyuneun Seo works across computer vision research, edge deployment, robotics-adjacent simulation, validation tooling, and backend/cloud delivery. The primary framing is engineering evidence and systems thinking, not a generic academic homepage.

Claims must remain factual. The site must not imply real-robot operation, real-flight deployment, or closed-loop robot control when the available evidence only supports simulation, research, or software deployment work.

## Information architecture

- Home (`/`): short positioning statement, capability tags, selected engineering projects, research snapshot, and clear links to CV/GitHub/LinkedIn.
- Projects (`/projects/`): collection-driven cards and detail pages for ETRI GNSS-denied localization, Jetson/Hailo edge deployment, ROS2/Gazebo Safe Landing, reusable C#/WPF validation tooling, and backend/cloud/CI-CD work.
- Publications (`/publications/`): real publication titles and venues only; include award information only where confirmed.
- CV (`/cv/`): concise Markdown CV using verified education, experience, skills, and publications.
- About (`/about/`): short engineering biography and current multimodal/facial-coordination research direction.

Template sample pages, talks, teaching entries, and placeholder posts should not appear in navigation or public content unless supported by real user data.

## Visual and technical direction

- Keep Academic Pages/Jekyll and its existing collection model.
- Use a restrained light theme with dark text, one technical accent color, compact cards, and strong whitespace.
- Make projects the first substantial content after the hero.
- Preserve static-site performance: no new frontend framework, no heavy runtime dependencies, and no unnecessary external assets.
- Ensure mobile layout, keyboard focus, readable contrast, and stable links.

## Data policy

- Replace all Academic Pages placeholder identity, education, social links, CV, portfolio, and publication metadata.
- Do not invent dates, metrics, employers, repository URLs, paper titles, venues, or awards.
- Use the existing project context and repository files as the source of truth; leave an item out when the facts cannot be verified.

## Implementation and verification

1. Update `_config.yml`, navigation, author profile, and SEO metadata.
2. Replace the home page and add the project collection content/layout needed for project-first presentation.
3. Replace placeholder CV and publication files with verified content.
4. Remove or hide sample pages/content from navigation and generated collections.
5. Add focused responsive styling without rewriting the Academic Pages theme.
6. Build the site locally with the repository's supported Jekyll workflow.
7. Preview the rendered home, projects, publications, and CV pages and check for broken links, placeholder text, layout overflow, and factual overclaiming.
