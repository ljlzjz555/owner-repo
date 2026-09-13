---
name: ecommerce-image-workflow
description: Build ecommerce product-image generation workflows, including brief intake, shot planning, prompt packs, channel-specific variants, and QA for marketplace or social commerce assets.
metadata:
  short-description: Ecommerce product image workflow
---

# Ecommerce Image Workflow

Use this skill when the user wants to plan, generate, revise, or systematize ecommerce product images for listings, ads, marketplace pages, livestream commerce, or social commerce.

The skill should produce a workflow that turns product information into commercially useful image outputs: clear product presentation, platform-ready dimensions, prompt packs, variant batches, and a quality-control loop. It should not replace brand, legal, or marketplace approval; keep claims and regulated content conservative unless the user supplies approved copy.

## Default Outcome

For most requests, deliver:

- A compact creative brief with assumptions called out.
- A shot list grouped by funnel role: hero, feature, lifestyle, comparison, detail, offer, and retargeting when relevant.
- Generation prompts with negative prompts or avoidance notes.
- Variant logic for audience, channel, season, offer, colorway, and localization.
- A QA checklist covering product accuracy, text, claims, compliance, composition, and export specs.

When the user asks for actual images, use an available image-generation tool for bitmap output. When they ask for a reusable process, prompt library, or team workflow, provide structured instructions and templates instead of generating images immediately.

## Intake

Collect only the missing details that materially affect output. If the user gives a product photo, product page, SKU sheet, brand guide, or prior campaign, use it as the source of truth.

Ask for clarification before generating if any of these are unknown and consequential:

- Product category and exact SKU or variant.
- Required channel or marketplace.
- Whether the image must match a real product photo exactly.
- Any prohibited claims, restricted ingredients, model usage constraints, or trademark issues.
- Required language, locale, dimensions, or file format.

If missing details are not blocking, proceed with clearly labeled assumptions and leave editable placeholders.

Read [references/brief-intake.md](references/brief-intake.md) when the task needs a reusable intake form, SOP, or handoff template.

## Image Planning

Plan images by commercial job rather than by decoration. Prioritize the product being recognizable, correctly scaled, and easy to understand in the first second.

- Hero images should isolate the product and make the offer or category obvious.
- Feature images should show one concrete benefit per image.
- Lifestyle images should show the product in a plausible use context without hiding key product details.
- Comparison images should avoid unverifiable superiority claims unless the user provides approved evidence.
- Detail images should highlight materials, texture, packaging, ingredients, controls, ports, fit, or included accessories.

Read [references/image-spec.md](references/image-spec.md) when the task needs detailed shot specs, prompt structure, or QA criteria.

## Channel Variants

Fit the workflow to the distribution surface. Dimensions, text density, safe areas, and claim tolerance change by channel.

- Marketplace listing images should favor clarity, exactness, white or clean backgrounds, and minimal text unless allowed.
- Paid social ads can use stronger hooks, lifestyle context, offer framing, and audience-specific variants.
- Short-video thumbnails need larger subjects, high contrast, and fewer words.
- Storefront or landing-page images can carry more brand atmosphere while keeping product details inspectable.

Read [references/channel-playbooks.md](references/channel-playbooks.md) when the user names a platform, campaign type, or batch export requirement.

## Prompt Packs

When writing prompts, separate product facts from creative direction so teams can review and reuse them.

Use this shape:

```text
Product facts:
<verifiable product details, dimensions, packaging, colors, included items>

Commercial goal:
<listing clarity, feature education, ad hook, seasonal offer, etc.>

Scene and composition:
<camera, background, props, lighting, product placement, safe area>

Style controls:
<brand tone, realism level, color palette, model rules, text rules>

Avoid:
<incorrect variants, extra logos, unsupported claims, distorted packaging, unreadable text>

Output:
<aspect ratio, dimensions, file format, number of variants>
```

Prefer batches that change one variable at a time when the user wants testing. For example, keep product and composition stable while varying audience, hook, background color, or offer.

## QA And Revision

Before finalizing, check:

- Product identity: shape, color, packaging, label, accessories, and scale match the source.
- Commercial clarity: the image communicates one job quickly.
- Text: spelling, language, contrast, safe area, and marketplace allowance.
- Claims: no invented certifications, discounts, medical effects, or performance promises.
- Composition: product is not cropped badly, blocked by props, or visually confused with competitors.
- Export: size, ratio, background, transparency, naming, and batch organization match the request.

When revising generated images, diagnose the failure in product facts, composition, style, or compliance terms, then change the smallest prompt section needed.
