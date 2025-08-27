---
# Leave the homepage title empty to use the site title
title: ''
date: 2024-01-24
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      # Avatar customization
      avatar:
        size: medium  # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: skills
    content:
      title: Skills
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '2'
  - block: experience
    content:
      title: Research Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Research Software Engineer
          company: University of Glasgow
          company_url: 'https://www.gla.ac.uk'
          company_logo: org-uofg
          location: Glasgow
          date_start: '2024-11-01'
          date_end: ''
          description: |2-
              * Working as part of Research Software Engineering Team
              * Developing FAIR and open source software
              * Working using agile software engineering techniques
        - title: Research Associate
          company: University of Glasgow
          company_url: 'https://www.gla.ac.uk'
          company_logo: org-uofg
          location: Glasgow
          date_start: '2023-03-05'
          date_end: '2024-10-31'
          description: |2-
              * Working on Large NIHR funded projects, to aid in evidence synthesis.
              * Development of web applications using R Shiny to aid in advance evidence synthesis techniques.
              * Working as part of a team, collaborating through multiple channels including GitHub / Jira
        - title: Technician
          company: University of Glasgow
          company_url: 'https://www.gla.ac.uk'
          company_logo: org-uofg
          location: Glasgow
          date_start: '2020-11-01'
          date_end: '2021-12-31'
          description: |2-
              * Working on an STFC funded grant to deliver a Findable Accessible Interoperable Reusable (FAIR) Data Pipeline
              * Producing opensource APIs in multiple programming languages (C++, Python, R, Julia, Java)
              * Working as part of a team collaborating using source control i.e., GIT and GitHub
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: 
          date_end: ''
          date_start: '2016-10-26'
          description: ''
          icon: org-uh
          organization: University of Herfortshire
          organization_url: https://herts.ac.uk
          title: University Prize - Outstanding Perfomance
          url: ''
    design:
      columns: '2'
  #- block: collection
  #  id: posts
  #  content:
  #    title: Recent Posts
  #    subtitle: ''
  #    text: ''
  #    # Choose how many pages you would like to display (0 = all pages)
  #    count: 5
  #    # Filter on criteria
  #    filters:
  #      folders:
  #        - post
  #      author: ""
  #      category: ""
  #      tag: ""
  #      exclude_featured: false
  #      exclude_future: false
  #      exclude_past: false
  #      publication_type: ""
  #    # Choose how many pages you would like to offset by
  #    offset: 0
  #    # Page order: descending (desc) or ascending (asc) date.
  #    order: desc
  #  design:
  #    # Choose a layout view
  #    view: compact
  #    columns: '2'
  #- block: portfolio
  #  id: projects
  #  content:
  #    title: Projects
  #    filters:
  #      folders:
  #        - project
  #    # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
  #    default_button_index: 0
  #    # Filter toolbar (optional).
  #    # Add or remove as many filters (`filter_button` instances) as you like.
  #    # To show all items, set `tag` to "*".
  #    # To filter by a specific tag, set `tag` to an existing tag name.
  #    # To remove the toolbar, delete the entire `filter_button` block.
  #    buttons:
  #      - name: All
  #        tag: '*'
  #      - name: Deep Learning
  #        tag: Deep Learning
  #      - name: Other
  #        tag: Demo
  #  design:
  #    # Choose how many columns the section has. Valid values: '1' or '2'.
  #    columns: '1'
  #    view: showcase
  #    # For Showcase view, flip alternate rows?
  #    flip_alt_rows: false
  #- block: markdown
  #  content:
  #    title: Gallery
  #    subtitle: ''
  #    text: |-
  #      {{< gallery album="demo" >}}
  #  design:
  #    columns: '1'
  - block: collection
    id: featured

title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        Use this area to speak to your mission. I'm a research scientist in the Moonshot team at DeepMind. I blog about machine learning, deep learning, and moonshots.

        I apply a range of qualitative and quantitative methods to comprehensively investigate the role of science and technology in the economy.
        
        Please reach out to collaborate 😃
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    id: software
    content:
      title: Software
      filters:
        folders:
          - software
    design:
      columns: '2'
      view: compact
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Please contact me through the University of Glasgow
      # Contact (add or remove contact options as necessary)
      #email: test@example.org
      #phone: 888 888 88 88
      #appointment_url: 'https://calendly.com'
      address:
        street: MVLS Shared Research Facilities, B3.08, Joseph Black Building
        city: Glasgow
        postcode: 'G12 8QQ'
        country: Scotland
        country_code: UK
      directions: Enter Building and Report to Reception
      office_hours:
        - 'Monday to Friday 09:00 to 17:00'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '55.872157'
        longitude: '-4.292951'  
      #contact_links:
      #  - icon: x-twitter
      #    icon_pack: fab
      #    name: DM Me
      #    link: 'https://twitter.com/RyanJField'
      #  - icon: skype
      #    icon_pack: fab
      #    name: Skype Me
      #    link: 'skype:echo123?call'
      #  - icon: video
      #    icon_pack: fas
      #    name: Zoom Me
      #    link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      #form:
      #  provider: netlify
      #  formspree:
      #    id:
      #  netlify:
      #    # Enable CAPTCHA challenge to reduce spam?
      #    captcha: false
    design:
      columns: '2'
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Easily build anything with blocks - no-code required!
        
        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
