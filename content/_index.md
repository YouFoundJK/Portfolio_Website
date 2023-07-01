---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    # id used to correlate the menu entries
    id: about
    content:
      title: Hi!
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
    design:
      background:
        gradient_end: '#3E3347'
        gradient_start: '#4D3F59'
        text_color_light: true
   
#  - block: features
#    content:
#      title: Skills
#      items:
#        - name: R
#          description: 90%
#          icon: r-project
#          icon_pack: fab
#        - name: Statistics
#          description: 100%
#          icon: chart-line
#          icon_pack: fas
#        - name: Photography
#          description: 10%
#          icon: camera-retro
#          icon_pack: fas

  - block: portfolio
    id: projects
    content:
      date_format: Jan 2006
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Plasma Physics
          tag: Plasma
        - name: Computational Physics
          tag: Computational
        - name: Condensed Matter
          tag: condensed
        - name: Mathematical Physics
          tag: math
        - name: 2D Heterostructures
          tag: hetero
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false

  - block: experience
    id: experience
    content:
      date_format: Jan 2006
      title: Experience
#      filters:
#        folders:
#          - experience
      items:
        - title: Research Student
          company: KIT
          company_url: 'https://www.kit.edu/index.php'
          company_logo: kitlogo
          location: Karlsruhe, Germany
          date_start: '2022-07-01'
          date_end: '2022-12-01'
          description: Master's Thesis on Designing twisted Bilayer Graphene Devices under Dr. Romain Danneau, INT.
        - title: Project Student
          company: TIFR
          company_url: 'https://www.tifr.res.in/'
          company_logo: tifrlogo
          location: Mumbai, India
          date_start: '2019-06-01'
          date_end: '2020-12-31'
          description: NIUS project on Theory of unconventional superconductivity under Prof. Rajdeep Sensarma.
          
        - title: Research Student
          company: HBCSE
          company_url: 'https://www.cbs.ac.in/'
          company_logo: hbcse
          location: Mumbai, India
          date_start: '2019-06-29'
          date_end: '2019-06-01'
          description: NIUS camp invited to learn under some of the best researchers as well as have hands-on experience on some of the state-of-art instruments and experimental techniques.
    design:
      columns: '2'
            
  - block: accomplishments
    id: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      # title: 'Accomplish&shy;ments'
      title: 'Certification'
      subtitle: 'Come on buddy lets do it'
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: ''
          date_end: '2021-07-01'
          date_start: ''
          description: 'Broad introduction to modern machine learning, including supervised learning (multiple linear regression, logistic regression, neural networks, and decision trees), unsupervised learning (clustering, dimensionality reduction, recommender systems), among others.'
          organization: Stanford University | Coursera
          organization_url: https://www.coursera.org
          title: Machine Learning
          url: 'https://www.coursera.org/learn/machine-learning'
        
        - certificate_url: https://www.coursera.org/account/accomplishments/certificate/L9KBH2VY52EP
          date_end: '2020-10-01'
          date_start: '2020-09-02'
          description: 'Generic mathematically rich introduction to the celebrated theory.'
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Introduction into General Theory of Relativity
          url: 'https://www.coursera.org/learn/general-relativity'
    
        - certificate_url: https://www.coursera.org/account/accomplishments/certificate/U77BPL78U67E
          date_end: '2021-03-01'
          date_start: '2021-01-01'
          description: Formulated informed blockchain models, hypotheses, and use cases.
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Stochastic processes
          url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
    
        - certificate_url: https://www.datacamp.com
          date_end: '2020-12-21'
          date_start: '2020-07-01'
          description: ''
          organization: DataCamp
          organization_url: https://www.datacamp.com
          title: 'Object-Oriented Programming in R'
          url: ''
    design:
      columns: '2'

#  - block: markdown
#    content:
#      title: Gallery
#      subtitle: ''
#      text: |-
#        {{< gallery album="demo" >}}
#    design:
#      columns: '1'
    
#  - block: collection
#    id: featured
#    content:
#      title: Featured Publications
#      filters:
#        folders:
#          - publication
#        featured_only: true
#    design:
#      columns: '2'
#      view: card

#  - block: collection
#    content:
#      title: Recent Publications
#      text: |-
#        {{% callout note %}}
#        Quickly discover relevant content by [filtering publications](./publication/).
#        {{% /callout %}}
#      filters:
#        folders:
#          - publication
#        exclude_featured: true
#    design:
#      columns: '2'
#      view: citation
#  - block: collection
#    id: talks
#    content:
#      title: Recent & Upcoming Talks
#      filters:
#        folders:
#          - event
#    design:
#      columns: '2'
#      view: compact

  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
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
      view: compact
      columns: '2'
  
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
        Feel free to leave a message and get in touch
      # Contact (add or remove contact options as necessary)
#      email: test@example.org
#      phone: 888 888 88 88
#      appointment_url: 'https://calendly.com'
#      address:
#        street: 450 Serra Mall
#        city: Stanford
#        region: CA
#        postcode: '94305'
#        country: United States
#        country_code: US
#      directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
#      office_hours:
#        - 'Monday 10:00 to 13:00'
#        - 'Wednesday 09:00 to 10:00'
#      contact_links:
#        - icon: twitter
#          icon_pack: fab
#          name: DM Me
#          link: 'https://twitter.com/Twitter'
#        - icon: skype
#          icon_pack: fab
#          name: Skype Me
#          link: 'skype:echo123?call'
#        - icon: video
#          icon_pack: fas
#          name: Zoom Me
#          link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id: youfoundjk@gmail.com
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
          
    design:
      columns: '2'
---
