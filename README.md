# SEO, AEO & GEO Starter Kit

An open-source collection of web development templates, structured data schemas, and optimization checklists designed to help developers and site owners optimize websites for **Search Engine Optimization (SEO)**, **Answer Engine Optimization (AEO)**, and **Generative Engine Optimization (GEO)**.

---

## Why This Project Exists

Traditional SEO starter kits focus mainly on basic meta tags and keywords. As search shifts toward AI answer engines and large language models (LLMs), websites need clean semantic HTML, explicit entity relationships, and machine-readable structured data. This repository provides lightweight, copy-pasteable resources to make modern web projects discoverable across both traditional search engines and AI-driven answer platforms.

---

## What's Inside (Roadmap & Current Modules)

- **Technical SEO Checklist:** Core HTML structure, meta tags, canonicalization, and crawlability standards.
- **AEO (Answer Engine Optimization) Templates:** Direct-answer formatting blocks, Q&A HTML patterns, and `FAQPage` JSON-LD schemas for featured snippets and voice/AI answers.
- **GEO (Generative Engine Optimization) Guidelines:** Citation-friendly content structures, entity clarity, and authoritative data formatting for LLM retrieval.
- **JSON-LD Schema Boilerplates:** Ready-to-use `Organization`, `Article`, `WebSite`, and `FAQPage` structured data snippets.

---

## Quick Start: Essential AEO/GEO Schema Template

Drop this JSON-LD snippet into the `<head>` of an FAQ or informational page to help search and answer engines parse your Q&A pairs cleanly:

```html
<script type="application/ld+json">
{
  "@context": "[https://schema.org](https://schema.org)",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "What is Answer Engine Optimization (AEO)?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Answer Engine Optimization (AEO) is the practice of structuring web content and schema markup so AI assistants and search engines can extract direct, accurate answers."
      }
    },
    {
      "@type": "Question",
      "name": "How does Generative Engine Optimization (GEO) differ from traditional SEO?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "While traditional SEO focuses on ranking links in search results, GEO focuses on entity clarity, verifiable facts, and structured context so generative AI models cite your content accurately."
      }
    }
  ]
}
</script>
