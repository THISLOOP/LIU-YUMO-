---
name: ip-quanan-skil1
description: Create complete Chinese brand IP plans and character-IP systems from a user-provided seed image and user-provided attributes to launch. Use when the user asks for 品牌IP全案, IP形象策划, 吉祥物/虚拟角色全案, IP设定, 从0到1打造IP, 基于一张图扩展IP, IP结合场景, IP场景主视觉, IP视觉资产流程, IP商业化落地, 小红书/社媒IP内容运营, or wants to turn a reference image into a reusable brand character strategy, 16:9 scene key visual, production workflow, prompts, deliverables, and iteration plan.
---

# IP全案skill

## Overview

Use this skill to build a complete brand IP case from strategy to execution. Treat an IP as a business-facing character system, not just a cute image: it must carry brand positioning, audience emotion, recognizable visual symbols, repeatable asset production, application scenarios, and ongoing content operations.

Default assumption: the user will provide one seed image as the visual mother image and may also provide attributes such as 亲子类, 科技感, 户外, 甜品, 教育, 美妆, 潮流, 城市, or 治愈. Base expansion, scenes, outfits, 3D conversion, actions, posters, and application mockups on the seed image's character identity plus those attributes. Do not invent a new mascot from scratch when a seed image is available.

Default to Chinese deliverables unless the user requests another language.

Seed-image intake gate: when the user directly provides or drops a seed image and asks to generate an IP case/images, do not start image generation immediately unless the required creative controls are already present in the user's message or prior same-task context. First ask the user to confirm these four items: (1) IP name, (2) overall IP style/direction, (3) proposal layout tone: dark layout or light/bright layout, and (4) desired typography style. Ask in one concise Chinese message and wait for the user's reply before generating. Suggested wording: `我先确认4个点再生图：1. IP名字叫什么？2. 整体风格想走什么方向？3. 排版想用深色还是浅色/亮色？4. 字体想要什么风格，默认黑体/粗黑体可以吗，还是想要楔线/宋体/书法感/其他？` If the user says to use your judgment, choose a fitting name/style/tone/font system and state those choices before generating. If the user has already answered some items, ask only for the missing items.

Default first image rule: the first generated image must be a horizontal 16:9 scene key visual showing the IP integrated into a scene derived from the IP's own traits and the user's attributes. The IP must have a clear body action and interact with the scene; do not let the character merely stand still as a static display model. Make this first image feel like a strong cover/key visual, not a sparse scene photo: the character and title typography should fill the composition, the scene can be moderately richer and more immersive, and the foreground subject must stay clear. For the first image only, the allowed elements are the character, the scene, the character's action/interaction, and the IP title/name typography. A huge low-opacity IP name or theme word may sit behind the character as a background typographic layer when the cover needs stronger visual impact. Do not add thumbnails, color swatches, detail cards, stickers, metadata blocks, page numbers, product modules, decorative panels, or extra UI-like proposal elements.

Default second image rule: the second generated image must be a horizontal 16:9 IP inspiration analysis board. It explains where the IP inspiration comes from by extracting elements from the seed character's traits, such as species/prototype, symbolic objects, material, color, accessories, and emotional cues. Use a clean layered collage layout: right side shows the same IP in a dynamic break-frame action pose; left/middle shows overlapping inspiration element cards, circles, arrows, and short English labels. Keep it visual-first with little text, and avoid torn-paper, ripped-edge, or messy scrap effects.

Default third image rule: the third generated image must be a horizontal 16:9 flat 2D three-view design board. It shows the same IP in clean orthographic front, side, and back views, with consistent scale and modeling-friendly details.

Default fourth image rule: the fourth generated image must be a horizontal 16:9 3D three-view design board. It shows the same IP in rendered front, side, and back views, matching the flat three-view proportions and seed-image identity.

Style fidelity rule: match the seed image's visual dimension and medium unless the user explicitly asks for conversion. If the seed image is flat 2D illustration, generate flat 2D follow-up assets. If the seed image is a 3D model/render/toy, generate 3D follow-up assets with matching material, lighting, and volume. Do not turn a 3D seed character into a 2D illustration or a 2D seed character into a 3D render by default.

After the first 16:9 scene key visual, second 16:9 inspiration analysis board, third 16:9 flat three-view board, and fourth 16:9 3D three-view board, the next useful page is usually a horizontal 16:9 six-expression/action grid: six full-body expressions/actions with short Chinese labels and minimal object links. Do not add an upper character profile/introduction section unless the user explicitly asks for it.

After the expression/action grid, a strong next step is to generate two separate horizontal 16:9 seasonal or holiday scene fusion visuals. Do not rely on a reference image being available. Select two fitting themes from Chinese/traditional holidays, commercial holidays, and seasons, such as Spring Festival, Dragon Boat Festival, Children's Day, Women's Day, Valentine's Day, Christmas, spring, summer, autumn, or winter. The choice must come from the IP's own traits and the user's brand tone. Each image should place the same IP in the foreground and a simple related scene behind it, with clear character-scene interaction and the same high-quality visual style as the approved preview. Follow each page's specified aspect ratio; use 3:4 only for extra vertical IP boards/character sheets/proposal visuals and 9:16 for Xiaohongshu/Douyin covers unless the user asks otherwise.

Scene differentiation rule: before generating the first 16:9 scene key visual and the two later 16:9 seasonal/holiday scene fusion visuals, define a three-scene map for pages 01, 06, and 07. These three pages must be visibly different in at least setting/location, time or atmosphere, interaction action, prop focus, and title wording. Do not let all three become variations of the same street corner, record shop, vending machine, neon alley, forest, candy land, studio, or other repeated environment. Page 01 may use the IP name as the main cover title. Pages 06 and 07 must use scene/theme English titles as the main title, not the IP name; the IP name can appear only as small metadata, packaging text, or be omitted.

The final showcase page can be a horizontal 16:9 IP merchandise display with a horizontal silver metal shopping basket. Keep it curated rather than crowded: show a realistic plush toy, blind box, a few mini figures, sticker sheet, phone case/pouch, scarf/gloves, and one or two charms/magnets. Include variants from previous expression and outfit systems when useful, so the merchandise family does not repeat only one base pose. The basket must be silver/chrome/light gray metal, not red.


Desktop output rule: when generating IP proposal images, save the final user-facing files directly into a Desktop folder named `[IP名称]IP全案`, for example `/Users/fuzzy/Desktop/MIMOIP全案`. If the image generation tool first creates files in an internal generated_images directory, immediately copy or export the approved/generated PNGs into this Desktop folder. Name every file clearly with page number, IP name, and page purpose. Recommended naming: `01_[IP名称]_场景主视觉.png`, `02_[IP名称]_灵感来源解析.png`, `03_[IP名称]_平面三视图.png`, `04_[IP名称]_三维三视图.png`, `05_[IP名称]_表情动作六宫格.png`, `06_[IP名称]_[场景英文标题].png`, `07_[IP名称]_[场景英文标题].png`, `08_[IP名称]_周边展示.png`, and `09_[IP名称]_竖版汇总展板.png` when a vertical consolidation board is made. Sanitize characters that are unsafe for file paths, such as `/`, `:`, or newline, by replacing them with `_`. Report the Desktop folder path after generation.

Vertical consolidation board rule: when the user says to delete/remove all horizontal pages or put all horizontal-page content into one vertical board, treat this as a layout/compositing step using the approved horizontal images. Do not regenerate or redesign the IP content unless the user explicitly asks. Arrange the existing horizontal images into a tall vertical proposal board with consistent margins and spacing. Do not add a new top title, content index, IP profile block, explanatory labels, extra captions, page numbers, badges, or new text modules unless the user explicitly asks for those additions. The goal is a clean vertical image-only compilation: directly place the provided horizontal pages in order, preserving their original typography and content as much as possible.

Global layout style rule: when the user provides IP proposal/layout references, extract their layout DNA and apply it consistently across all default visuals. Treat these references as typography, spacing, hierarchy, and page-system guidance only; never copy their character, brand, logo, exact words, or scene content. First identify the reference's title logic, text placement, panel rhythm, color/accent system, caption density, and image-module structure, then prepend that layout system to every image prompt. Do not assume the proposal must be black or dark just because one reference is dark. If the user has not clearly chosen a layout tone, ask one short confirmation before generating the full case: `整体排版想偏深色还是浅色？`

For the current preferred reference direction, use an editorial/cyber IP proposal language when it fits the IP. In dark mode, use black or very dark textured backgrounds, subtle grain/noise, large rounded 16:9 image panels, strong Chinese/English title hierarchy, small corner metadata, selective oversized semi-transparent English words behind hero images, neon/cyan/purple/magenta or IP-derived accents, and small detail thumbnails/cards. In light mode, translate the same structure into white, pale gray, cream, pastel, or brand-color backgrounds with soft shadows, clean rounded panels, strong title hierarchy, low-opacity oversized background words, and IP-derived accents. Keep it premium and unified, but preserve each page's function. The first scene key visual is the cover exception: it may use a huge low-opacity IP name/theme word behind the character to fill the composition, but it must not include thumbnails, swatches, metadata blocks, or analysis cards. Technical three-view pages must remain clean and readable, expression grids must stay uncluttered, and scene visuals should not be covered by decorative type.

Text layout rule: use concise visual-first typography. A page can use Chinese primary title with English subtitle, English primary title with small Chinese support, or bilingual quote/caption depending on purpose. Use one main title, one small subtitle/caption, and a few labels only. Avoid long paragraphs, dense microtext, random text placement, and text that covers the IP's face, body, product details, or scene interaction.
Typography consistency rule: before generating a series, define one unified font system and keep it consistent across every horizontal page and any final vertical board. The default core font should be bold black-style sans serif / 黑体 / geometric grotesk, because it is clean, commercial, and suitable for most IP proposal pages. Use the same Chinese title font family, English title font family, label font family, weight logic, outline/shadow/glow/bevel treatment, spacing, and capitalization rules on every generated image in the series. If a title uses glow, outline, extrusion, italic slant, metal texture, or cyber/neon effect, the same treatment logic should appear consistently across all pages rather than only one page. For IPs with classical, cultural, historical, calligraphy, Guochao, museum, heritage, or ancient-style attributes, the unified system may switch from black-style sans serif to one serif/wedge-serif/calligraphic title family such as Songti/Ming-style, wedge-serif, engraved serif, or seal-inspired display type, but it must still remain one consistent family system across the whole series. Do not mix unrelated fonts page by page, do not alternate playful rounded, cyber, serif, handwritten, and condensed styles randomly, and do not let generated pages invent new title fonts unless the user explicitly changes the typography direction.

## Core Workflow

Follow the SCALE structure:

1. **S - Strategy 品牌策略定位**
   - If the user only provides a seed image and asks to generate, pause before image generation and collect the four creative controls: IP name, overall IP style/direction, dark vs light/bright layout tone, and typography style. Ask only for missing items, then proceed after the user's reply.
   - Define brand background, product category, target audience, price band, brand tone, and competitive context.
   - Identify the user's emotional need: healing, companionship, confidence, rebellion, luck, professionalism, humor, status, belonging, or decompression.
   - Read the user's provided attributes and decide the scene direction they imply, such as parent-child outdoor play, cloud candy land, mountain adventure, future technology lab, beauty dressing room, campus, city commute, or forest festival.
   - For seasonal/holiday scene visuals, select two themes that fit the IP and brand tone from options such as Spring Festival, Dragon Boat Festival, Children's Day, Women's Day, Valentine's Day, Christmas, spring, summer, autumn, and winter. Do not choose themes randomly; explain the fit through the IP's symbols, personality, material, audience, and emotional value.
   - Before generating pages 01, 06, and 07, write a compact scene differentiation map: page number, scene name, location, time/atmosphere, main interaction action, prop focus, and title text. Confirm the three scene concepts are not visually interchangeable before prompting image generation.
   - If the user provides layout/style references, define one global proposal layout system before generating images. Use it to unify all pages without overriding the character identity or each page's required purpose.
   - Define one typography system at the same time as the global layout system: default to bold black-style sans serif / 黑体 for commercial, tech, cute, trendy, parent-child, beauty, food, and most modern IPs; use one consistent serif/wedge-serif/calligraphic title system only when the IP has clear classical, cultural, historical, or Guochao attributes. Apply the same font family logic, title effects, weights, spacing, and label style to every generated page.
   - If the overall layout tone is unclear, ask one concise confirmation before generating the full case: `整体排版想偏深色还是浅色？` Use the user's answer to decide dark-mode or light-mode proposal pages.
   - Decide the IP role: mascot, spokesperson, social content protagonist, sales assistant, membership icon, collectible, or campaign character.
   - Produce one sentence positioning: `一个为[人群]提供[情绪/价值]的[角色类型]。`

2. **C - Character 角色设定**
   - Choose a role prototype: human, animal, plant, food, object, monster, spirit, abstract emotion, local culture symbol, or product-derived character.
   - Define personality with tension. Good IP characters need contrast, such as `嘴硬但温柔`, `社恐但可靠`, `可爱但反骨`, `专业但不端着`.
   - Create 1-3 visual memory points: silhouette, eyes, headwear, gesture, color, prop, texture, symbol, or body proportion.
   - Identify 1-3 scene interaction hooks: what the IP can naturally touch, hold, discover, decorate, protect, plant, gift, eat, race, guide, or celebrate in a scene.
   - Define constraints: avoid competitor similarity, unsafe cultural symbols, overused styles, and hard-to-produce details.

3. **A - Asset 视觉资产生产**
   - Before generating any default visual from a newly provided seed image, confirm the IP name, overall IP style/direction, dark vs light/bright proposal tone, and typography style unless those controls are already known from the current task.
   - Save final user-facing image outputs into `/Users/fuzzy/Desktop/[IP名称]IP全案` by default, not only inside internal generated_images folders. Use clear page-numbered filenames for every horizontal page and vertical board, and copy generated tool outputs there immediately after each image is created.
   - Start from the user-provided seed image whenever available. Extract and lock the character's silhouette, face, proportions, color logic, key accessories, style, and mood.
   - If no seed image is provided and image generation is requested, ask the user for one seed image unless they explicitly allow a text-only original concept.
   - Apply the global layout style to every default visual when one is provided: shared margins, title zones, panel rhythm, label style, page numbering/metadata, accent colors, and image-card treatment. For the first scene key visual, apply only the cover mood, title/name typography, and optional huge low-opacity background word; do not add analysis modules, thumbnails, swatches, page numbers, metadata blocks, or decorative cards.
   - Generate the first visual as a horizontal 16:9 IP scene key visual. The scene must come from the IP's visual traits and the user's attributes, not from a generic background. The IP must perform a clear action and interact with the scene, not simply stand still.
   - Generate the second visual as a horizontal 16:9 IP inspiration analysis board. Extract inspiration elements from the seed image and IP traits; show them as clean overlapping visual cards on the left/middle, with the same IP breaking out of a clean frame in an action pose on the right.
   - Build a clean 2D base body on a white background only after the seed image identity is clear.
   - Build clothing/skin systems from brand scenes, products, seasons, campaigns, occupations, and user lifestyles.
   - Convert stable 2D designs into 3D/C4D/Octane-style renders when the use case needs posters, toys, high-end visual impact, or campaign materials.
   - Use action transfer to create expressive poses from reference photos or described scenes.
   - Generate the third visual as a horizontal 16:9 flat 2D three-view board after the inspiration analysis board. It should show the same IP in front, side, and back views, with clean orthographic setup and consistent scale.
   - Generate the fourth visual as a horizontal 16:9 3D three-view board after the flat three-view board. It should show matching rendered front, side, and back views using the seed image's material language.
   - After the two three-view boards, create a horizontal 16:9 six-expression/action grid when the user wants a proposal-style next page: six full-body actions, short Chinese labels, and one small prop or object-linked situation per action.
   - After the expression/action grid, create two separate horizontal 16:9 seasonal/holiday scene fusion visuals. Each visual should use one selected theme, a simplified scene, foreground/middle/background separation, and a clear action that makes the IP interact with the environment.
   - For the final showcase, create one horizontal 16:9 curated merchandise display using a horizontal silver shopping basket and a restrained set of IP products, including selected expression/outfit variants as product SKUs.
   - Create follow-up IP boards, multi-angle views, expression packs, vertical social covers, and material-ready deliverables after the first scene visual, inspiration board, and two three-view boards are approved.

4. **L - Launch 应用落地**
   - Map IP assets to real touchpoints: social avatar, stickers, comments, Xiaohongshu posts, Douyin covers, packaging, cards, store displays, event standees, web/app UI, PPT, membership systems, and merchandise.
   - Use the inspiration analysis board as a proposal page that explains why the IP looks this way, helping clients understand and remember the visual logic before production assets.
   - Prioritize high-frequency scenarios first: chat stickers, social posts, product packaging, bag charms/keychains, desktop items, and campaign posters.
   - Use the two 16:9 seasonal/holiday scene visuals as campaign key visuals, banner assets, poster crops, launch teasers, seasonal social content, and scene-based story starters.
   - Use the final silver-basket merchandise showcase as a pitch image for retail display, SKU planning, launch bundles, blind-box systems, gift sets, and IP commercialization pages.
   - Turn the IP into recurring content columns rather than one-off graphics.

5. **E - Evaluate 评估迭代**
   - Check recognition: can users identify it without the logo?
   - Check brand association: does the character naturally point back to the brand?
   - Check extensibility: can it change clothes, poses, scenes, emotions, and products?
   - Check inspiration clarity: can viewers understand the IP's source logic through enlarged visual elements without reading long text?
   - Check scene fit: do the selected seasonal/holiday themes feel natural for this IP, and does the character actually interact with the scene rather than being pasted onto a background?
   - Check scene differentiation: are pages 01, 06, and 07 clearly different in setting, time/atmosphere, background modules, interaction action, prop focus, and main title? If they look like the same scene with minor changes, regenerate pages 06 and/or 07 with a new scene concept.
   - Check visual quality: does the output maintain the seed image's medium, high-quality render/illustration style, simplified background, shallow depth of field when appropriate, and clear foreground subject separation?
   - Check layout continuity: do all default pages feel like one proposal deck, with consistent dark/light layout tone, title placement, bilingual logic, margins, panel styling, metadata, accent colors, typography system, font effects, weights, and label style?
   - Check first-cover impact: does the first scene key visual feel like a strong cover, with character/action/title typography filling the composition rather than feeling sparse?
   - Check merchandise clarity: is the basket silver, horizontal, and readable; are there enough SKUs to show commercialization without overcrowding; do expression and outfit variants make the product family feel expandable?
   - Check shareability: would users save, repost, comment with, wear, or gift it?
   - Check commercialization: can it become packaging, gifts, blind boxes, plush, charms, collaborations, membership assets, or offline displays?

## Reference-Inspired Production Flow

When the user provides visual references like Xiaohongshu screenshots or creator workflows, extract reusable production logic, not the exact character design. When the user provides a seed character image, treat that image as the identity source and expand from it. When the user provides attributes, use them to infer the world around the IP. The default production pipeline is:

`母图识别 -> 属性理解 -> 场景推导 -> 全局版式风格锁定 -> 16:9场景主视觉 -> 16:9灵感来源解析页 -> 16:9平面三视图页 -> 16:9三维三视图页 -> 16:9六宫格表情动作页 -> 两张16:9节日/季节场景融合图 -> 16:9银色购物篮周边展示 -> 前期准备 -> 替换服装 -> 2D转3D -> 动作迁移 -> 展板/海报排版 -> 多角度转换 -> 应用落地`

Use this as a practical execution path:

0. **母图识别**
   - Inspect the user-provided image first.
   - Extract fixed identity: species/prototype, outline, head-body ratio, face, eyes, mouth, hairstyle/head feature, accessories, core colors, material, line style, rendering dimension (2D or 3D), and emotional tone.
   - Separate fixed traits from expandable traits. Fixed traits must remain stable across all generated images.
   - Identify whether the seed is a flat 2D image or a 3D model/render. Keep this dimension stable in follow-up outputs unless the user explicitly asks for 2D-to-3D or 3D-to-2D conversion.
   - If the seed image is blurry, cropped, or ambiguous, state the uncertainty and make the smallest reasonable assumption before expanding.

1. **属性理解**
   - Read the user's attribute words as scene constraints, not decoration.
   - Convert attributes into visual world rules. Examples: `亲子类` means safe, warm, playful, family-friendly, park/home/learning scenes; `科技感` means clean light, screens, soft futurism, devices, lab/city interfaces; `甜品` means clouds, cream, candy, pastries, pastel softness; `户外` means hills, forest, road, sky, sun, adventure props.
   - Combine attributes with IP traits. A monkey should naturally enter mountains/forest/adventure; a cotton-candy IP should enter sweet clouds/cream/pastel sky; a bee-like IP should enter flowers/garden/sunshine; a beauty doll should enter makeup mirror/dressing room/editorial stage.

2. **场景推导**
   - Before generating, write or mentally define: `IP是什么 -> 它来自哪里 -> 它适合做什么 -> 它和用户属性如何合并 -> 第一张场景主视觉是什么`.
   - For series that include pages 01, 06, and 07, define all three scene concepts together before generating them. Avoid repeating the same core setting, same background objects, same camera distance, same color-lighting mood, and same character action across the three scene visuals.
   - Make the IP interact with the scene through action, props, scale, lighting, and story. Avoid simply placing a cutout character on a background.
   - Use a broad 16:9 composition with foreground, middle ground, background, and clear breathing room for title/logo if needed.

2.5. **全局版式风格锁定**
   - If the user provides proposal/layout references, extract a reusable page system before image generation: background tone, panel shape, title placement, bilingual title logic, subtitle/caption density, metadata position, accent colors, thumbnail/card modules, spacing, and typography system.
   - Lock one typography system before generating the series. Specify the Chinese font direction, English font direction, title weight, label weight, effect treatment, and whether the system is modern black-style sans serif or culture-led serif/wedge-serif. Keep this typography identical across the 16:9 pages and any vertical consolidation board.
   - If the reference shows a dark style but the user has not confirmed the overall tone, ask whether the proposal should use dark layout or light layout. Do not automatically copy black backgrounds.
   - For dark layout, use dark textured backgrounds, high-contrast typography, neon/metal accents, and low-opacity oversized background words where appropriate.
   - For light layout, keep the same typography and panel rhythm but use pale, white, cream, pastel, or brand-color backgrounds, soft shadows, airy spacing, and low-opacity oversized background words where appropriate.
   - Apply this system to all default pages so the output feels like one IP proposal deck, not unrelated images.
   - Treat font consistency as part of the page system: all titles, subtitles, labels, metadata, and decorative typography should look like they come from one design kit.
   - For the current editorial reference style, use large rounded panels, bold bilingual headings, selective oversized low-opacity background words, and compact detail cards on pages that need them. Use IP-derived accent colors instead of blindly copying the reference palette.
   - Keep functional pages clear: three-view pages may use a dark outer frame but should keep the character-view area white, pale, or studio-clean; expression/action pages should remain readable; scene pages should prioritize the IP-scene interaction over typography.
   - Avoid copying reference logos, exact names, exact slogans, characters, watermarks, and specific scenes.

3. **16:9场景主视觉**
   - The first generated image must be horizontal 16:9.
   - Show the IP as the protagonist inside its fitting world, with enough cover-level visual fullness. Avoid outputs that look too sparse, empty, or like a simple clean scene photo.
   - Give the IP a clear body action: jumping, reaching, holding, planting, decorating, discovering, racing, resting, pouring, pushing, pulling, hugging, waving, guiding, or another action that fits the scene and brand tone.
   - Make the action and scene interact. The IP should touch, hold, use, discover, decorate, or affect something in the environment rather than pose in front of it.
   - Keep the seed image identity stable while allowing only scene-essential props, costume details, supporting small objects, and cover typography.
   - Use visual references like character campaign posters: sunny hills for cheerful outdoor IP, forest trail for monkey/adventure IP, sweet clouds for dessert IP, futuristic interface for technology IP.
   - Keep the background lower-detail than the character but not necessarily empty. Use shallow depth of field, soft blur, foreground/middle/background depth, and reduced detail so the IP clearly separates from the environment.
   - Include the IP name as a tasteful title/logo lockup, usually in the upper-left. If the upper-left is visually busy, place it in another calm negative-space area. Keep text minimal and readable.
   - For stronger cover impact, allow a huge low-opacity IP name or theme word behind the character. It should fill space and create hierarchy while staying behind the subject and never covering the face or key body details.
   - Do not include anything beyond the IP, the scene, the action/interaction, and the IP title/name typography. Do not add detail thumbnails, color swatches, side cards, analysis modules, page numbers, metadata labels, product callouts, extra stickers, or decorative UI panels on this first image.

4. **16:9灵感来源解析页**
   - The second generated image must be a horizontal 16:9 inspiration analysis board.
   - Use this page to explain the IP's visual origin and creative logic before showing the technical three-view board.
   - Derive inspiration elements from the seed image and the IP's own traits, not from a random reference. Typical sources include species/prototype, object analogy, symbolic motifs, facial features, accessories, color, texture/material, and emotional cues.
   - For example, an alien-cat IP can be decomposed into `cat-ear silhouette`, `alien signal`, `starry eyes`, `star antenna`, `orbit collar`, and `soft vinyl/plush material`; a hawthorn IP can connect fruit skin, pointed leaves, candy shell, and sour-sweet feeling.
   - Use a clean layered collage layout rather than a rigid grid. Left/middle areas can use overlapping rounded cards, translucent panels, enlarged crops, circle highlights, arrows, and short labels.
   - Place the same IP on the right side as a large hero character with a dynamic break-frame action pose. It can jump, float, reach, step out, wave, or lean out of a clean rounded frame.
   - Use English only by default on this page. Keep text minimal: one title, one short subtitle, and brief element labels. Avoid long paragraphs.
   - Avoid torn-paper, ripped-edge, paper scraps, excessive shards, or messy scrapbook effects. The break-frame effect should use clean borders, soft shadows, glows, translucent frames, or rounded panels.
   - Match the seed image's medium: if the seed is 2D, make the board 2D; if the seed is 3D, make the board 3D with matching toy/render material.

5. **16:9平面三视图页**
   - The third generated image must be a horizontal 16:9 flat 2D three-view design board.
   - Show the same IP in three clean orthographic angles: front view, side view, and back view.
   - Keep the seed image identity locked across all three views: silhouette, head-body ratio, face, eyes, mouth, head features, accessories, colors, material language, and fixed marks.
   - Make the page modeling-friendly: simple lines, even scale, light guide lines, white or pale background, minimal labels, no scene background.
   - Use flat 2D concept/setup style even when the seed is 3D, because this page is for clear structure and modeling reference. Do not invent new details while flattening.
   - Include only necessary labels such as `平面三视图`, `正视图`, `侧视图`, `后视图`, and optional `MASCOT DESIGN / [IP名称]`.
   - Do not add 3D renders, scene backgrounds, extra characters, name-typography interaction, long copy, story paragraphs, or decorative asset modules on this page.

6. **16:9三维三视图页**
   - The fourth generated image must be a horizontal 16:9 3D three-view design board.
   - Show the same IP in three rendered angles: front view, side view, and back view.
   - Match the third image's flat three-view proportions and details as closely as possible.
   - Keep the seed image identity locked across all three views: silhouette, head-body ratio, face, eyes, mouth, head features, accessories, colors, material language, and fixed marks.
   - Make the 3D views toy-like and presentation-ready: C4D/soft vinyl/plush material as appropriate, consistent scale, soft lighting, simple gradient or clean studio background.
   - Include only necessary labels such as `三维三视图`, `正视图`, `侧视图`, `后视图`, and optional `MASCOT DESIGN / [IP名称]`.
   - Do not add scene backgrounds, extra characters, long copy, story paragraphs, or unrelated asset modules on this page.

7. **16:9六宫格表情动作页**
   - Use this as the natural next page after the 16:9 scene key visual, 16:9 inspiration analysis board, 16:9 flat three-view board, and 16:9 3D three-view board, especially when the user asks for expressions, stickers, actions, emotion packs, or a proposal-style follow-up page.
   - The page should be horizontal 16:9 unless the user asks otherwise.
   - Do not include an upper character profile/introduction section, IP keyword area, color swatches, or long English paragraph by default. Add those only if the user explicitly asks for a character profile page.
   - Use the reference page only for expression/action logic, spacing, and commercial neatness. Do not copy the reference character or its exact graphic assets.
   - Keep the current seed image as the identity source. Lock the character's silhouette, face, eyes, body proportion, color logic, accessories, and emotional tone.
   - Match the seed image's medium: if the seed is 2D, make the six actions 2D; if the seed is 3D, make the six actions 3D with matching toy/render material.
   - Create exactly six expression/action stickers unless the user asks for a different number. Arrange them in a clean horizontal 2 x 3 grid or another simple six-cell layout that fits 16:9.
   - Use short Chinese labels under each action by default, such as `开心`, `大笑`, `哭泣`, `尴尬`, `寻找`, `爱心`.
   - Each expression must use a full-body pose plus a related small object, prop, symbol, or situation.
   - Avoid expression packs that only change eyes, eyebrows, mouth, or head angle. The character should interact with objects such as a gift, crescent pillow, raindrop cloud, tiny planet, magnifying glass, map, heart, sparkle, phone, product, food, bag, flower, sign, or brand-relevant prop.
   - Keep decoration restrained. Use at most one small related prop or a few tiny supporting symbols per action; avoid busy doodles, excessive motion lines, dense stars, or decorative clutter.
   - Useful starter emotions/actions: happy, laughing, crying, embarrassed, searching, love, greeting, cheering, sleepy, angry, shocked, comforting, inviting, selling, and celebrating.
   - Use clean commercial proposal composition: white or pale background, clear spacing, minimal labels, and no dense explanatory text.

8. **两张16:9节日/季节场景融合图**
   - Use this as the natural next step after the six-expression/action grid, especially when the user wants scene extension, seasonal content, holiday campaign visuals, or IP world-building.
   - Generate two separate horizontal 16:9 images. Do not combine them into one board unless the user asks.
   - Compare both later scene visuals against the first 16:9 scene key visual before prompting. Pages 06 and 07 must not reuse page 01's exact main environment, background modules, title logic, or character-scene action. If page 01 is a night street / record shop / vending machine scene, choose clearly different later settings such as rooftop secret-message scene, indoor bedroom/desk scene, transit station, festival stall, park, snow window, toy room, gallery display, product table, or another setting that fits the IP.
   - Page 06 and page 07 title rule: the main title must be the scene/theme English title, not the IP name. Examples: `VALENTINE STREET PASS`, `SUMMER STREET MIX`, `WINTER WINDOW SIGNAL`, `SPRING FIELD GUIDE`, `DRAGON BOAT PICNIC`. The IP name may appear only as a small metadata label, packaging detail, or tiny logo-safe mark.
   - Do not depend on reference images. If references are provided, extract only the general logic of simple character-scene fusion, lighting, and depth; do not copy the exact scene, character, text, watermark, or composition.
   - Select two themes from a fixed theme pool: Spring Festival, Dragon Boat Festival, Children's Day, Women's Day, Valentine's Day, Christmas, spring, summer, autumn, and winter. Choose the two that best match the IP's own traits and brand tone.
   - Build scene concepts from `IP特性 + 节日/季节主题 + 情绪价值`. Example: an alien-cat with star antennae can fit spring star meadow, winter star holiday night, Children's Day toy room, or Valentine's Day glowing heart planet; a food IP can fit Dragon Boat Festival picnic or autumn harvest; a parent-child IP can fit Children's Day playroom or spring park.
   - Keep the same IP identity locked and match the seed image's medium. If the seed is 2D, generate 2D scene visuals; if the seed is 3D, generate 3D scene visuals with matching toy/render material.
   - Each image must show the IP in the foreground and a simple scene behind it. The IP must interact with the scene through a clear action: planting, watering, decorating, discovering, gifting, holding, racing, resting, protecting, guiding, or celebrating.
   - Keep the scene simple and commercially clean. Use shallow depth of field, soft blur, foreground/middle/background separation, and background detail lower than the character detail.
   - Preserve high visual quality: polished campaign visual, coherent lighting, soft cinematic/studio render, crisp foreground subject, clean composition, no messy text, no watermark.
   - Avoid big background typography, pure layout panels, unrelated props, dense festival clutter, and decorative scenes that do not connect to the IP.

9. **16:9银色购物篮周边展示**
   - Use this as the final commercialization/showcase page when the user asks for an IP derivative product display, merchandise basket, retail bundle, SKU family, or final product presentation.
   - Generate one horizontal 16:9 image. Do not make it vertical.
   - The central prop must be a horizontal silver metal shopping basket: silver, chrome, light gray, or polished wire metal. Do not use a red, orange, yellow, or colorful basket.
   - Use a clean dark or neutral studio background and high-quality commercial product photography/render lighting.
   - Keep the merchandise curated and breathable rather than crowded. Aim for about 7-9 main product groups, not dozens of small objects.
   - Recommended product mix: one hero plush toy, one blind box package, three mini vinyl/rubber figures, one sticker sheet, one phone case or pouch, one scarf/neck warmer or gloves, and one or two magnets/keychains/charms.
   - Include expression and outfit variants from earlier IP assets when useful: a happy expression mini figure, an explorer/pilot/guardian outfit mini figure, expression stickers, or seasonal/holiday product graphics. This prevents the showcase from repeating only one base mascot.
   - Keep all products in the same IP system: consistent colors, eyes, star antennae or signature marks, packaging language, and material logic.
   - Maintain a clear hierarchy: hero plush near center, packaging and phone accessory behind or to the side, mini figures along the front edge, soft goods grouped together, small charms/magnets used sparingly.
   - Avoid visual fatigue: leave negative space, avoid filling every gap, avoid too many labels, and do not scatter many tiny items.

10. **前期准备**
   - Build or summarize a simple 2D base character from the seed image.
   - Specify head-body ratio, body shape, face, hair/head feature, accessories, and fixed marks.
   - Use original references only for inspiration. Never copy a creator's exact character.

11. **替换服装**
   - Use clothing references to generate brand-fit outfits.
   - Preserve the character's base face, silhouette, color logic, and white/clean background.
   - Treat outfits as a scalable "skin system" for holidays, campaigns, products, and communities.

12. **2D转3D**
   - Convert the stable 2D character to a 3D render for richer presence.
   - Control material language: skin, fabric, hair, plastic, ceramic, metal, soft vinyl, plush.
   - Use high-resolution output when the visual will be used in posters or presentation decks.

13. **动作迁移**
   - Either use a pose reference image or describe the desired pose clearly.
   - Maintain character identity strictly: same face, same eyes, same proportions, same outfit unless intentionally changing skin.
   - Use action sets tied to real IP functions: greeting, explaining, guiding, selling, celebrating, comforting, teasing, warning, or inviting.

14. **场景化**
   - Place the IP in environments that support the brand story: store, product scene, city street, desk, package, exhibition, festival, online interface, or user life scene.
   - Avoid empty atmospheric backgrounds unless the brand genuinely needs a cinematic campaign poster.
   - For the first scene key visual, keep it horizontal 16:9. For later social covers, use 9:16; for IP boards and character sheets, use 3:4.

15. **展板/海报排版**
   - Turn strong character scenes into poster layouts with headline, slogan, campaign copy, and logo-safe space.
   - Keep type aligned with the brand tone: premium, playful, trendy, professional, local, youth, or healing.
   - For the first key visual, use horizontal campaign composition. For follow-up boards, use vertical board logic: title/top area, large character hero area, asset modules below, application mockups at the bottom.

16. **多角度转换**
   - Generate front, side, back, 3/4, top-down, low-angle, full-body, half-body, standing, sitting, and key pose views as needed.
   - Use these for style guides, animation, 3D modeling, merchandise, and consistency checks.

## Deliverable Menu

Choose deliverables based on the user's scope. For a first draft, include the essentials:

- Brand IP strategy diagnosis
- Audience and emotion map
- IP role and one-sentence positioning
- Character name options
- Character story and personality
- Visual keywords and memory points
- Seed image identity analysis
- Attribute-to-scene analysis
- Global proposal layout style extraction when references are provided
- First 16:9 IP scene key visual prompt
- Second 16:9 IP inspiration analysis board prompt
- Third 16:9 flat 2D three-view board prompt
- Fourth 16:9 3D three-view board prompt
- Fifth 16:9 six-expression/action grid prompt
- Sixth and seventh 16:9 seasonal/holiday scene fusion prompts
- Final 16:9 silver shopping basket merchandise showcase prompt
- Vertical image-only consolidation board layout when the user wants approved horizontal pages placed into one vertical board
- Desktop output folder and page-numbered PNG filenames: `/Users/fuzzy/Desktop/[IP名称]IP全案/01_[IP名称]_场景主视觉.png` through the final vertical board when generated
- Base character prompt from the seed image
- Outfit/skin system
- Expression/action library plan
- 2D/3D production prompt templates
- Vertical scene poster plan
- Social content column ideas
- Application touchpoint list
- Commercialization directions
- Iteration checklist

For a full case, add:

- Competitive IP differentiation
- Naming rationale
- Tone of voice
- Relationship map or supporting characters
- Brand color/material guidance
- Three-view/multi-angle requirements based on the seed image
- Packaging and merchandise map
- Launch campaign rhythm
- Xiaohongshu/Douyin content calendar
- KPI and feedback mechanism

## Prompting Rules

When writing image-generation prompts for IP work:

- Before writing image-generation prompts from a newly provided seed image, make sure four controls are known: `IP名称`, `整体风格`, `深色/浅色或亮色排版`, and `字体风格`. If any are missing and the user has not delegated the choice, ask first and wait.
- Always reference the user-provided seed image when available. State that it is the identity source.
- Always lock the character identity: name, species/prototype, head-body ratio, face shape, eyes, fixed accessories, signature colors, body proportions, and expression style.
- Separate what must stay consistent from what can change.
- Specify output purpose: first 16:9 scene key visual, second 16:9 inspiration analysis board, third 16:9 flat 2D three-view board, fourth 16:9 3D three-view board, fifth 16:9 expression/action grid, base design, outfit transfer, 3D render, action transfer, scene poster, expression pack, product mockup, or multi-angle sheet.
- Match the seed image's medium by default: 2D seed produces 2D assets; 3D seed produces 3D assets. Only convert dimensions when the user explicitly asks.
- If the user provides layout/style references, extract and apply one global proposal layout style across all default images. Describe it as `全局版式风格` in prompts, including title placement, Chinese/English hierarchy, background tone, panel shape, metadata/corner labels, accent colors, image-module rhythm, and a locked typography system.
- Always specify a `字体系统` for the whole series. Default: unified bold black-style sans serif / 黑体 / geometric grotesk for Chinese and English headings, with consistent weights, spacing, capitalization, and effects. For classical/cultural/Guochao IPs, use one consistent serif/wedge-serif/calligraphic title direction instead. The chosen typography and text effects must remain the same across every generated horizontal page and any final vertical board.
- If the user has not specified the overall layout tone, ask whether the proposal should use `深色排版` or `浅色排版` before generating the full set. Do not assume black/dark backgrounds from a single reference.
- When using an editorial/cyber proposal style, specify either `深色颗粒质感背景` or `浅色/品牌色干净背景` based on the user's choice, plus `圆角大图面板、强标题层级、中英结合标题、选择性使用半透明英文大字背景`. Use small corner metadata and detail cards only on pages where they are useful; do not add them to the first scene key visual.
- For the first generated image, specify `横版16:9，IP与场景融合主视觉`. For each later default page, follow its specific aspect ratio. Use `竖版3:4` only for extra vertical IP boards/posters or `竖版9:16` for social covers.
- For the first 16:9 key visual, specify `IP必须有明确动作并与场景互动；人物和标题文字共同撑满画面；可使用低透明大号IP名称/主题词放在人物后面；场景可适度丰富但主体清晰、前后景分离；除IP、场景、动作、标题/IP名称排版外，不要信息卡、色卡、缩略图、页码、元信息或UI模块`.
- For the second 16:9 inspiration analysis board, specify `横版16:9，灵感来源解析页；右侧IP破框动作；左侧/中部叠加式灵感元素卡片；英文少量标签；不要规整表格；不要碎纸撕裂效果；不要长文`.
- For the third flat 2D three-view board, specify `横版16:9，平面三视图；只包含正视图、侧视图、后视图；建模友好；不要3D渲染，不要场景背景，不要长文说明`.
- For the fourth 3D three-view board, specify `横版16:9，三维三视图；只包含正视图、侧视图、后视图；比例匹配平面三视图；3D/C4D/潮玩/软胶材质；不要场景背景，不要长文说明`.
- For the six-expression/action grid, specify `横版16:9，只保留六个表情/动作，不要上方人物介绍区；中文标签；每个表情必须关联一个小物体或道具；装饰少；不要只改五官`.
- For the pair of seasonal/holiday scene fusion visuals, specify `生成两张独立横版16:9；从春节、端午节、儿童节、女神节、情人节、圣诞节、春夏秋冬中选择两个最适合IP的主题；先和第01张场景主视觉做差异检查，确保第01/06/07三张场景在地点、时间氛围、角色动作、道具焦点、标题文字上明显不同；第06/07主标题写场景英文标题，不要写IP名；前景是同一IP，后方是简洁场景；角色必须与场景互动；保持高质量画质、浅景深、背景柔和虚化、主体清晰分离；不要大字排版`.
- For the final merchandise showcase, specify `横版16:9，横置银色金属购物篮，不要红色篮子；周边数量克制，约7-9组核心单品；包含毛绒、盲盒、小胶人、贴纸、手机壳/包、围脖/手套、少量冰箱贴/钥匙扣；可加入表情和服装变体；留白充足，不要堆满`.
- Specify background needs: white background for asset extraction; real scene for campaign posters; transparent background when needed for stickers.
- Specify material only when useful: soft vinyl, plush, C4D, Octane render, ceramic, fabric texture, toy-like, matte plastic, glossy plastic, CG skin, or paper-cut illustration.
- Include negative constraints when consistency matters: do not change eyes, do not change head shape, do not add extra limbs, do not add text unless requested, do not imitate a referenced artist exactly.

Use this compact prompt pattern:

```text
基于用户提供的[母图/参考图]，生成[用途]。
前置确认：[如果用户只给母图就要求生成，先确认IP名称、整体风格、深色/浅色或亮色排版、字体风格；缺哪项问哪项，用户回复后再生成]。
必须保持：[固定身份特征]。
IP名称：[名称]。
用户属性：[亲子类/科技感/甜品/户外/美妆等]。
场景推导：[根据IP特征和用户属性推导出的世界]。
场景差异检查：[如果生成第01/06/07三张场景图，先写清三张各自的地点、时间氛围、互动动作、道具焦点和主标题；三张必须明显不同，不能都像同一个背景换姿势；第06/07主标题必须是场景英文标题，不要用IP名做主标题]。
可以变化：[服装/动作/场景/材质]。
全局版式风格：[先确认或推定深色/浅色排版；如果用户提供版式参考，写清统一背景、标题位置、中英标题关系、圆角面板、角标信息、缩略图/卡片模块、色彩点缀；若无参考，则使用干净商业提案版式]。
字体系统：[整套统一字体。默认使用粗黑体/黑体/geometric grotesk 作为核心字体；中文标题、英文标题、标签、角标、页码使用同一字体家族逻辑和统一字重；若使用描边、发光、斜体、金属、立体、霓虹等效果，每一页都保持同一种处理；古风/文化/国潮/历史属性IP可统一改用宋体/明体/楔线体/书法感标题字体，但全系列必须一致；不要每张图换一种字体]。
风格：[2D插画/3D C4D Octane/潮玩/毛绒/品牌海报]。
画面要求：[第一张横版16:9；IP必须有明确动作并与场景互动；封面感要强，人物和标题文字共同撑满画面；可使用低透明大号IP名称/主题词放在人物后面；场景适度丰富但主体清晰分离；不加色卡/缩略图/角标元信息/解析卡/装饰模块；第二张横版16:9灵感来源解析页，右侧IP破框动作，左侧叠加灵感元素；第三张横版16:9平面三视图页；第四张横版16:9三维三视图页；第五张横版16:9六宫格表情动作页；后续横版16:9或竖版9:16、背景、构图、清晰度、是否留白]。
限制：[不要改变角色核心特征，不要照抄参考，不要多余文字]。
```

When the user wants the whole case to follow an editorial proposal layout, first ask or infer whether it should be dark or light. Then add the matching global layout block to each image prompt:

```text
全局版式风格：整套IP提案保持统一的潮流编辑版式；根据用户确认使用深色或浅色排版。深色版使用黑色/深灰颗粒质感背景和高对比光效；浅色版使用白色/浅灰/奶油色/品牌浅色背景和柔和阴影。页面边缘留出稳定边距；使用大圆角16:9主图面板或模块卡片；标题采用中英结合，中文可做主标题，英文做小副标题，或用英文粗体词作为半透明背景层；点缀色从IP主色中提取。
字体系统：整套IP提案必须使用同一套字体系统。现代/潮流/科技/亲子/甜品/美妆/商业IP默认使用粗黑体/黑体/geometric grotesk，中文标题、英文标题、标签、角标和页码保持同一字体家族逻辑、统一字重和统一字距；如果主标题使用霓虹发光、描边、斜体、立体、金属或阴影效果，所有页面按同一规则处理。古风/文化/国潮/历史属性IP可统一切换为宋体/明体/楔线体/书法感标题字体，但仍要全系列一致。不要每张图混用不同字体风格。
文字限制：视觉优先，文字少而准；不要长段正文，不要密集小字，不要遮挡角色脸部、三视图、商品细节或场景互动；不要复制参考图的具体品牌名、logo、角色、标语和水印。
功能保护：第一张场景主视觉允许低透明大号IP名称/主题词作为背景标题字，但只允许IP、场景、动作/互动、标题/IP名称排版，不加缩略图、色卡、页码、元信息、解析卡或装饰模块；三视图页允许外框承接整体版式，但角色展示区必须干净清晰；六宫格保持可读和留白；节日/季节场景不要被大字排版压过主体。
```

For the first scene key visual, use:

```text
基于用户提供的母图，生成第一张横版16:9 IP场景融合主视觉。
必须保持母图角色的核心身份：[轮廓/脸/眼睛/比例/颜色/配饰/风格]。
IP名称：[名称]。
用户提供的IP属性：[属性词]。
根据IP特性和属性推导场景：[例如小猴子在山林探险、棉花糖在甜甜云朵里、科技IP在柔和未来实验室、亲子IP在阳光公园/家庭互动场景]。
动作要求：IP必须有明确身体动作，并且动作要和场景发生关系，例如跳跃、伸手、抱住、推开、拉动、浇灌、发现、装饰、驾驶、奔跑、躺卧、递送、守护、倒饮料、举起场景中的核心道具等。不要只是站在那里。
封面增强要求：如果画面太空或用户希望更强视觉冲击，使用封面增强模式。让人物和标题文字共同撑满画面；人物可占画面45%-65%；使用一个巨大、低透明度的IP名称或主题词放在人物后方，部分被人物遮挡，不遮挡脸和关键身体结构；场景可比普通主视觉更丰富，有纵深和沉浸感，但所有场景细节必须服务于IP和动作。
画面要求：横版16:9，IP是主角，角色与场景发生互动，前景/中景/背景层次清楚；背景可以适度丰富但细节必须低于主体，主体清晰锐利，与背景明显分离；左上角或合适留白处可放置一个小IP名称，同时可在人物后方放置低透明大标题字。
第一张内容限制：除IP本体、场景、动作/互动、IP名称/标题排版之外，不要任何信息模块。不要色卡、缩略图、细节卡、角标元信息、页码、贴纸、产品模块、解析标签、图标装饰、边栏、UI面板或无关道具。
限制：不要做成普通展板，不要只是白底角色，不要让IP静态站桩，不要把IP贴在背景上，不要让背景抢主体，不要改变母图核心长相，不要堆长文。
```

For the second inspiration analysis board, use:

```text
基于用户提供的母图，生成第二张横版16:9 IP灵感来源解析页。
必须保持母图角色的核心身份：[轮廓/脸/眼睛/比例/颜色/配饰/风格]。
必须匹配母图媒介：[如果母图是二维平面插画，则生成二维平面；如果母图是3D模型/渲染/潮玩小模，则生成3D模型/渲染，不要转成二维]。
IP名称：[名称]。
灵感来源：从母图角色自身特征提取灵感元素，而不是随机发明。提取方向包括：[物种/原型]、[标志性轮廓]、[五官特征]、[配饰/符号]、[颜色]、[材质]、[情绪气质]、[相关物体]。
元素示例：[例如外星小猫 = 猫耳轮廓、外星信号、星空眼睛、星星触角、轨道围脖、软胶/毛绒材质；山楂IP = 山楂果实、糖壳、尖叶、酸甜口感、红色圆形]。
版式：横版16:9，右侧放同一个IP的大主形象，做动态破框动作，可以跳出、浮出、伸手、挥手、跨出干净圆角框；左侧/中部放灵感元素解析。
左侧设计：不要规整表格。使用叠加式视觉拼贴，但要干净高级：重叠圆角卡片、半透明面板、放大的局部特写、圆圈标注、箭头、少量星标或小图标。
文字要求：英文为主，少量即可。标题可用 `IP INSPIRATION` / `INSPIRATION PROFILE`，副标题一句短句，元素标签用短英文，如 `CAT EAR`、`ALIEN SIGNAL`、`STARRY EYE`、`STAR ANTENNA`、`ORBIT COLLAR`、`SOFT VINYL`。不要长段说明。
视觉要求：视觉为主、文字为辅；画面有设计感但不杂乱；干净、柔和、商业提案感；主体清晰，卡片层次清楚，配色跟IP一致。
限制：不要碎纸、不要撕纸边、不要纸屑、不要凌乱 scrapbooking 效果；不要规整网格表格；不要中文长文；不要照抄参考图角色；不要重新发明角色；不要做成三视图页或场景主视觉。
```

For the third flat 2D three-view board, use:

```text
基于用户提供的母图，生成第三张横版16:9 IP平面三视图设计页。
必须保持母图角色的核心身份：[轮廓/脸/眼睛/比例/颜色/配饰/风格]。
IP名称：[名称]。
版式：横版16:9，只做平面三视图，不做三维渲染。画面中并排展示同一IP的正视图、侧视图、后视图，比例一致，站姿/基准线一致。
风格：干净的2D设定稿/建模参考图风格，简单线条，色块清楚，轻微辅助线，白色或浅色背景。
要求：即使母图是3D，也要把结构转译为清晰的平面正侧后三视图，用于建模和比例说明，但不要重新发明角色细节。
文字要求：只保留必要标签，如“平面三视图”“正视图”“侧视图”“后视图”，右上角可放“MASCOT DESIGN / [IP名称]”。
限制：不要三维渲染，不要场景背景，不要正文说明，不要故事段落，不要多个角色，不要资产面板，不要改变母图核心长相。
```

For the fourth 3D three-view board, use:

```text
基于用户提供的母图，生成第四张横版16:9 IP三维三视图设计页。
必须保持母图角色的核心身份：[轮廓/脸/眼睛/比例/颜色/配饰/风格]。
必须参考第三张平面三视图的比例和固定细节：[正视图/侧视图/后视图的比例、轮廓、配饰、颜色、固定标记]。
IP名称：[名称]。
版式：横版16:9，只做三维三视图。画面中并排展示同一IP的3D正视图、3D侧视图、3D后视图，比例一致，站姿/基准线一致。
风格：3D/C4D/潮玩/软胶/毛绒等与母图匹配的材质语言，灯光柔和，背景简洁，像正式建模/潮玩展示页。
要求：三维图必须匹配平面三视图和母图身份，不要改眼睛、头型、比例、配饰、颜色、固定标记。
文字要求：只保留必要标签，如“三维三视图”“正视图”“侧视图”“后视图”，右上角可放“MASCOT DESIGN / [IP名称]”。
限制：不要平面线稿，不要场景背景，不要正文说明，不要故事段落，不要多个角色，不要资产面板，不要改变母图核心长相。
```

For the six-expression/action grid, use:

```text
基于用户提供的母图，生成第五张横版16:9 IP六宫格表情动作页。
必须保持母图角色的核心身份：[轮廓/脸/眼睛/比例/颜色/配饰/风格]。
必须匹配母图媒介：[如果母图是二维平面插画，则生成二维平面；如果母图是3D模型/渲染/潮玩小模，则生成3D模型/渲染，不要转成二维]。
IP名称：[名称]。
版式：横版16:9，只保留六个表情/动作，不要上方人物介绍区，不要英文简介，不要关键词，不要色块。白色或浅色干净背景，2x3六宫格，间距清楚，适配横版画面。
六个表情与中文标签：开心、大笑、哭泣、尴尬、寻找、爱心。
动作要求：每个表情都必须是同一IP的全身动作，并关联一个小物件/道具/情境。示例：开心配一个小星星或小礼物；大笑配一个月亮抱枕或捂肚动作；哭泣配一个小雨云或泪滴；尴尬配一个小星球或遮脸动作；寻找配放大镜和小地图；爱心配一个发光爱心。
装饰要求：整体简洁，不要过多装饰物；每格最多一个主要小道具和少量辅助符号。
文字要求：只用中文短标签，不用英文标签，不写长段说明。
限制：不要重新发明角色，不要照抄参考角色，不要只做大头表情，不要只改变眼睛眉毛嘴巴，不要堆长文，不要多个不同角色，不要把3D母图画成2D。
```

For the pair of seasonal/holiday scene fusion visuals, use:

```text
基于用户提供的母图，生成两张独立的横版16:9 IP节日/季节场景融合图。
必须保持母图角色的核心身份：[轮廓/脸/眼睛/比例/颜色/配饰/风格]。
必须匹配母图媒介：[如果母图是二维平面插画，则生成二维平面；如果母图是3D模型/渲染/潮玩小模，则生成3D模型/渲染，不要转成二维]。
IP名称：[名称]。
品牌调性/用户属性：[属性词]。
标题规则：第06/07节日或季节场景图的主标题必须写场景英文标题，不要用IP名称做主标题。IP名称只允许作为很小的角标、包装细节或不出现。例如主标题用 `VALENTINE STREET PASS`、`SUMMER STREET MIX`、`WINTER WINDOW SIGNAL`，不要写成 `[IP名称]`。
主题选择：不依赖参考图。从以下命题中选择两个最适合该IP和品牌调性的主题：春节、端午节、儿童节、女神节、情人节、圣诞节、春天、夏天、秋天、冬天。选择逻辑要来自IP特性、符号、材质、性格和情绪价值，不要随机选择。
场景差异要求：先对比第01张场景主视觉，再确定第06和第07两张场景。第01/06/07三张必须在地点、时间氛围、背景核心物、角色动作、道具焦点和标题文字上明显不同。不要连续使用同一类夜街、唱片店、自动贩卖机、霓虹墙、甜品云、森林、实验室、白底棚拍等相似场景。若两张后续场景或它们与第01张看起来像同一场景换角度，必须重新设计场景。
场景推导：为每个主题写出一个简单场景和互动动作。要求是“前景IP + 后方简洁场景”，角色必须与场景发生关系，例如种植/浇灌/发现/装饰/赠送/守护/玩耍/休息/庆祝。示例：外星小猫可选择春天星光草地，动作是浇灌发光星星种子；也可选择圣诞节窗边星星小树，动作是挂发光星星装饰。
第一张：[主题A]，横版16:9，[简洁场景]，[角色互动动作]。
第二张：[主题B]，横版16:9，[简洁场景]，[角色互动动作]。
画质要求：保持高质量商业IP场景主视觉效果；如果是3D母图，使用高品质3D玩具/软胶/C4D/Octane感渲染，柔和电影感光线，材质干净，眼睛高光清晰；如果是2D母图，保持同等精致的2D插画质感。主体清晰锐利，背景柔和虚化，浅景深，前景/中景/背景分离，画面干净，有温度，像正式品牌季节 campaign visual。
场景要求：背景比角色更简约，节日/季节元素少而准，不要堆满装饰；不要只把角色贴到背景上；不要大字排版，不要英文粗体字在后面，不要水印，不要截图UI，不要长文案。
限制：不要重新发明角色，不要改变母图核心长相，不要照抄参考图场景，不要让场景抢主体，不要把3D母图画成2D，不要把2D母图转成3D，除非用户明确要求转换。
```

For the final silver shopping basket merchandise showcase, use:

```text
基于用户提供的母图，生成一张横版16:9 IP衍生品银色购物篮展示图。
必须保持母图角色的核心身份：[轮廓/脸/眼睛/比例/颜色/配饰/风格]。
必须匹配母图媒介和商品质感：[如果母图是3D模型/潮玩小模，则周边展示使用高质量3D产品摄影/商业渲染；如果母图是二维平面插画，则商品上的图案保持二维IP视觉，但商品本身可以是真实产品摄影质感]。
IP名称：[名称]。
核心道具：横置银色金属购物篮，银色/铬色/浅灰金属线框，有真实金属高光。购物篮必须是银色，不要红色、橙色、黄色或其他彩色篮子。
画面尺寸：横版16:9，干净棚拍或深色/中性背景，商业产品摄影角度，光线柔和，主体清晰。
商品数量：整体要克制，不要堆满。使用约7-9组核心单品，留出呼吸感和负空间。
推荐商品组合：1个主毛绒玩具；1个盲盒包装；3个小胶人/软胶小摆件；1张表情贴纸；1个手机壳或小包；1组围脖/手套等软织物；1-2个冰箱贴/钥匙扣/亚克力挂件。
变体要求：可以融入前面已经生成过的不同表情和不同服装元素，例如开心/哭泣/寻找/爱心表情贴纸，宇宙探索者/飞行员/守护者服装小胶人，节日/季节图案包装。不要只重复同一个基础IP形象。
陈列要求：主毛绒放中间或视觉中心；盲盒、贴纸、手机壳/包放后侧或两侧；小胶人沿购物篮前缘排布；围脖/手套归为一组；少量挂件/磁贴点缀。层次清楚，不要散乱。
视觉要求：统一IP色系和包装系统，颜色可使用薄荷绿、薰衣草紫、星星黄、白色、银色；产品真实可售卖，材质区分清楚，如毛绒、软胶、纸盒、织物、亚克力、金属。
限制：不要竖版，不要红色购物篮，不要空篮子，不要堆太多小物，不要复制参考图角色，不要重新发明角色，不要截图UI，不要水印，不要大字排版，不要让周边密到审美疲劳。
```

For vertical IP boards, use:

```text
基于用户提供的母图或已经生成/提供的横版页面，制作一张竖版品牌IP展板。
如果用户已经提供横版页面，并且说“删掉横版”“横版内容放到竖版里”“先生成看看效果”，优先执行图片拼版：直接使用现有横版图，不重新生成角色，不改动横版图里的原始内容。
必须保持母图角色或现有横版页的核心身份：[轮廓/脸/眼睛/比例/颜色/配饰/风格/原有标题与版式]。
展板内容来源：[已提供的16:9场景主视觉、灵感来源、平面三视图、三维三视图、表情动作、节日/季节场景、周边应用等横版页面]。
版式要求：竖版长图或竖版展板；按横版页面顺序排列；第一张主视觉可跨整行放大，其余页面可两列排列，最后周边/总结页可跨整行；保持统一外边距、间距、黑底/浅底等既有提案风格；尽量完整保留每张横版图内容，少裁切。
文字规则：如果用户没有要求新增说明，竖版展板上不要额外添加顶部标题、内容索引、IP定位、说明段落、模块标签、页码、角标或新文案；直接放图片即可。只保留横版图内部原本已有的文字。
限制：不要重新发明角色，不要改变母图核心长相，不要把横版图内容重画歪，不要额外堆文字，不要把图片裁得过狠，不要加入与横版内容无关的装饰模块。
```

## Output Style

Write outputs like a strategist who can also direct visual production:

- Be concrete and usable, not just conceptual.
- Give names, slogans, prompts, assets, and rollout ideas when appropriate.
- Make assumptions explicit when the brand category or audience is unknown.
- When layout/style references are provided, first summarize the extracted global layout rules in 3-6 concise bullets, then apply those rules consistently to every default image prompt.
- After generating images, place all final files on the user's Desktop in a folder named `[IP名称]IP全案`; name each PNG with page number, IP name, and purpose, then report that absolute folder path.
- When the user directly drops an image and asks to generate an IP series, ask the four intake questions first unless already answered: IP name, overall style, dark/light layout tone, and typography style. Do not generate first and ask later.
- Before generating a full visual case, ask whether the user wants dark layout or light layout if that choice is not already clear from the user's words or references.
- Ask only the minimum needed questions; otherwise provide a strong first draft and mark it as adjustable.
- Prefer structured Chinese headings and concise bullets.

When the user asks to update this skill, edit the skill files directly and preserve the word `skill`.

