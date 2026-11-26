# Structured Data for the Chumbow Lab Portfolio Website

These JSON-LD examples are prepared for the portfolio website, not for insertion into GitHub Markdown. Publish them only after checking that the linked pages, visible identity and contact route are current.

## Person

~~~json
{
  "@context": "https://schema.org",
  "@type": "Person",
  "name": "Paul Chumbow",
  "url": "https://paulchumbow254.lovable.app/",
  "sameAs": [
    "https://www.linkedin.com/in/paul-chumbow",
    "https://github.com/chumbowlab"
  ],
  "email": "paulchumbow254@gmail.com",
  "knowsAbout": [
    "Founder support",
    "Digital operations",
    "WordPress",
    "Website maintenance",
    "Search engine optimisation",
    "Workflow design",
    "AI-assisted productivity"
  ]
}
~~~

## Chumbow Lab brand

Use Organization only if the portfolio presents Chumbow Lab as an identifiable professional studio/brand. This schema does not claim that Chumbow Lab is a registered company.

~~~json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "Chumbow Lab",
  "url": "https://paulchumbow254.lovable.app/",
  "sameAs": [
    "https://github.com/chumbowlab",
    "https://www.linkedin.com/in/paul-chumbow"
  ],
  "email": "paulchumbow254@gmail.com",
  "description": "A portfolio of practical web solutions, WordPress work, digital operations and workflow-focused projects."
}
~~~

## Publication checks

- Ensure the page visibly identifies Paul Chumbow and explains the Chumbow Lab brand.
- Ensure every listed service is supported by visible work or a clearly labelled area of focus.
- Validate the JSON-LD before deployment.
- Do not add aggregate ratings, reviews, awards, service prices or organisation registration details without evidence.
- Keep the page's visible content consistent with the structured data.