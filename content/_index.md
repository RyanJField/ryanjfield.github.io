---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-05-20
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      #button:
      #  text: Download CV
      #  url: uploads/resume.pdf
      headings:
        about: 'Research Summary'
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: resume-experience
    content:
      username: me
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
      css_class: "bg-gray-100 dark:bg-gray-800"
  - block: resume-skills
    content:
      title: Skills
      username: me
  - block: resume-awards
    content:
      title: Awards
      username: me
    design:
      css_class: "bg-gray-100 dark:bg-gray-800"
  #- block: markdown
  #  content:
  #    title: '📚 My Research'
  #    subtitle: ''
  #    text: |-
  #      Use this area to speak to your mission. I'm a research scientist in the Moonshot team at DeepMind. I blog about machine learning, deep learning, and moonshots.
#
  #      I apply a range of qualitative and quantitative methods to comprehensively investigate the role of science and technology in the economy.
#
  #      Please reach out to collaborate 😃
  #  design:
  #    columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 1
  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
      css_class: "bg-gray-100 dark:bg-gray-800"
  - block: collection
    id: software
    content:
      title: Recent Software
      text: ""
      filters:
        folders:
          - software
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - events
    design:
      view: article-grid
      columns: 2
      css_class: "bg-gray-100 dark:bg-gray-800 w-full"
  #- block: collection
  #  id: news
  #  content:
  #    title: Recent News
  #    subtitle: ''
  #    text: ''
  #    # Page type to display. E.g. post, talk, publication...
  #    page_type: blog
  #    # Choose how many pages you would like to display (0 = all pages)
  #    count: 10
  #    # Filter on criteria
  #    filters:
  #      author: ''
  #      category: ''
  #      tag: ''
  #      exclude_featured: false
  #      exclude_future: false
  #      exclude_past: false
  #      publication_type: ''
  #    # Choose how many pages you would like to offset by
  #    offset: 0
  #    # Page order: descending (desc) or ascending (asc) date.
  #    order: desc
  #  design:
  #    # Choose a layout view
  #    view: card
  #    # Reduce spacing
  #    spacing:
  #      padding: [0, 0, 0, 0]
  - block: contact-info
    content:
      title: Contact
      subtitle: Please contact me through the University of Glasgow
      visit_title: Office Address
      connect_title: Get in Touch
      address:
        lines:
          - MVLS Shared Research Facilities
          - B3.08
          - Joseph Black Building
          - Glasgow
          - G12 8QQ
      office_hours:
        - "Monday - Friday: 9:00 AM - 5:00 PM"
      email: ryan.field@glasgow.ac.uk
      phone: 
      social:
        - icon: brands/bluesky
          url: https://bsky.app/profile/ryanfield.me
        - icon: brands/github
          url: https://github.com/RyanJField
        - icon: brands/linkedin
          url: https://www.linkedin.com/in/ryan-field
        #- icon: custom/uofg-24
        #  url: https://www.gla.ac.uk/stafflist/search/person/4edeece28292/
        - icon: academicons/google-scholar
          url: https://scholar.google.com/citations?user=1hOmyCAAAAAJ
        - icon: academicons/orcid
          url: https://orcid.org/0000-0002-4424-9890
      map_url: https://maps.app.goo.gl/arSX72JQhYXJhgct5
      map_embed: |
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2238.459043649398!2d-4.295708223110905!3d55.87205147312853!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x488845d1cd2c0dd1%3A0x8c7b9ddabdd2ebd2!2sJoseph%20Black%20Building!5e0!3m2!1sen!2suk!4v1779205580769!5m2!1sen!2suk" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
      show_form: false
    design:
      #css_class: "bg-gray-50 dark:bg-gray-900"
      spacing:
        padding: ["3rem", 0, "3rem", 0]
  - block: cta-card
    demo: true # Only display this section in the HugoBlox Kit demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by HugoBlox Kit - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/kit" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/kit on GitHub">Star</a>

        Easily build anything with blocks - no-code required!

        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: 'bg-primary-300 dark:bg-primary-700'
        css_style: ''
---
