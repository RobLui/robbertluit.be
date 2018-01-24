---
title: Home
content:
    items: '@self.modular'
    order:
        by: default
        dir: asc
        custom:
            - _header
            - _services
            - _portfolio
            - _clients
menu: Home
googletitle: 'Portfolio Robbert Luit'
googledesc: 'My personal website. Contains a list of my skills and projects that I''ve made so far. Passionate in what I do. ## iDevelop ##'
twitterenable: true
twittercardoptions: summary
twittershareimg: /_header/rl_website.jpg
twittertitle: 'Portfolio Robbert Luit'
twitterdescription: 'My personal website. Contains a list of my skills and projects that I''ve made so far. Passionate in what I do. ## iDevelop ##'
articleenabled: false
musiceventenabled: false
orgaenabled: false
eventenabled: false
personenabled: false
restaurantenabled: false
restaurant:
    acceptsReservations: 'yes'
    priceRange: $
facebookenable: true
facebooktitle: 'Portfolio Robbert Luit'
facebookdesc: 'My personal website. Contains a list of my skills and projects that I''ve made so far. Passionate in what I do. #iDevelop#'
facebookauthor: 'Robbert Luit'
facebookimg: /home/_header/rl_website.jpg
onepage_menu: true
form:
    name: contact
    action: /home
    fields:
        -
            name: name
            label: Name
            classes: form-control
            placeholder: 'Enter your name'
            autofocus: 'off'
            autocomplete: 'on'
            type: text
            position: left
            validate:
                required: true
        -
            name: email
            label: Email
            classes: form-control
            placeholder: 'Enter your email address'
            type: email
            position: left
            validate:
                required: true
        -
            name: message
            label: Message
            placeholder: 'Enter your message'
            type: textarea
            classes: form-control
            position: right
            validate:
                required: true
    buttons:
        -
            type: submit
            classes: 'btn btn-primary btn-lg'
            value: Submit
    process:
        -
            email:
                subject: '[Site Contact Form] {{ form.value.name|e }}'
                body: '{% include ''forms/data.html.twig'' %}'
        -
            message: 'Thanks! We will be in touch soon :)'
---

