backend:
  name: git-gateway
  branch: main  # change if your main branch has a different name

media_folder: "images/uploads"
public_folder: "/images/uploads"

site_url: "https://elliotdonation.netlify.app"  # your site URL

collections:
  - name: "pages"
    label: "Pages"
    folder: ""
    create: true
    slug: "{{slug}}"
    fields:
      - { label: "Page Title", name: "title", widget: "string" }
      - { label: "Main Content", name: "body", widget: "markdown" }
      - { label: "Header Image", name: "header_image", widget: "image" }
      - { label: "Call to Action Button Text", name: "button_text", widget: "string", default: "Donate Now" }
      - { label: "Donation Link", name: "button_link", widget: "string", default: "https://elliotdonation.netlify.app" }
      - { label: "Premium Theme Color", name: "theme_color", widget: "color", default: "#6a1b9a" }
      - { label: "Accent Color", name: "accent_color", widget: "color", default: "#ffcc00" }
