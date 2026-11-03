# Examples
![[Baby Coloured.png|263]]![[baby.png|384]]
![[ComicBaby.png|373]]![[Baby Greyscale.png|245]]
# Guide
Sure — I can walk you through how to take a baby photo and recreate the dark, high-contrast, grainy, black-and-white “baby tomato” look from the video using GIMP. I’ll assume you already have the baby image you want to use and GIMP installed. If anything is unclear, tell me what version of GIMP you’re using and I’ll adapt.

Step-by-step workflow (GIMP)

1) Prepare your document
- Open GIMP and create a new document or open the baby photo (File > Open).
- If you want a white background like the video, create a new white layer below the baby layer: Layer > New Layer, fill with white, move under the baby layer.

1) Isolate the baby head (cutout)
- Use the Free Select Tool (lasso) or the Foreground Select Tool to roughly enclose the baby’s head.
- Refine selection: use Quick Mask (Shift+Q) to paint refinements with a soft brush (paint black to remove, white to add), then turn off Quick Mask to get the selection back.
- With the selection active, choose Layer > Mask > Add Layer Mask and select “Selection.” This non-destructively isolates the head. Alternatively, choose Select > Invert then press Delete if you want to remove the background permanently.

3) Convert to grayscale with high contrast
- Duplicate the isolated head layer (right-click layer > Duplicate) so you keep an original copy.
- Desaturate the duplicate: Colors > Desaturate > choose Luminosity (or try Average/Lightness and preview which looks best).
- Increase contrast: Colors > Levels — drag the black and white input sliders inward to deepen shadows and brighten highlights. Adjust the midtone (gamma) slider for the right balance.
- Optionally use Colors > Curves for finer control: create an S-curve to increase contrast while keeping some midtone detail.

4) Add darkened, stamped shading and stylized features
- Create a new transparent layer above the grayscale head set to “Multiply” (or “Overlay” depending on desired effect) to paint dark shading.
- Use a hard round or textured brush at medium opacity (20–50%) to paint darker areas like eye sockets, under the nose, around mouth edges, and hairline. This gives the more graphic, slightly shaded look from the video.
- For sharp dark elements (like heavy outlines), use a smaller hard brush on a separate layer. You can lower opacity to blend.
- To get that “subtle face integrated into tomato” feel, avoid full realistic shading — keep shapes simplified and slightly flattened.

5) Add halftone / grain / texture
- Grain (global): duplicate the final head layer, then go Colors > Components > Desaturate (if not already B/W). Then Filters > Noise > RGB Noise (or HSV noise) with low amounts to add speckle. Alternatively Filters > Noise > Hurl > choose small values. Set this noise layer to Overlay or Soft light and reduce opacity to taste.
- Film grain / grain map: create a new layer, fill with 50% gray (Edit > Fill with FG color after setting FG to 50% gray), then Filters > Noise > Hurl or Filters > Noise > Pick (if available) to add fine texture. Set layer mode to Overlay and lower opacity.
- Paper/grain paper texture: you can use built-in Paper patterns or open a scanned paper texture, put it above or below the head, set Mode to Multiply or Overlay and adjust opacity to give the distressed, tactile feel.
- For a heavy grainy print look use Filters > Artistic > Photocopy or Filters > Distorts > Newsprint (if available as plugin) to simulate dot/halftone patterns. Adjust settings and opacity.

6) Add dark lines / vine-like tangles (optional)
- Create a new transparent layer above the head. Use a thin, slightly textured brush and black color to paint slim tangled lines that mimic vine stems. Use the Path tool for smooth, editable curves (create path, stroke path with brush).
- Lower opacity or set layer mode to Multiply if you want them integrated.

7) Add distressed edges and poster texture
- Duplicate the entire composited group to a new layer and apply Filters > Artistic > Apply Canvas or Filters > Decor > Add Border if you want rough edges.
- Use Layer Mask on background to brush in subtle stains/roughness with a soft textured brush to match the distressed poster look.

8) Final global adjustments (levels, dodge/burn)
- Merge visible copies to a new layer (Select the topmost layer and choose Layer > New from Visible). Work non-destructively by duplicating first.
- Use Colors > Levels or Colors > Curves for final contrast tweak.
- Lightly dodge (brighten) or burn (darken) areas with the Dodge/Burn tool (exposure 5–15%) to emphasize key features.
- If you want a slightly warm/greenish tint in midtones for the calyx effect, you can add a Colorize layer clipped to the vine/calyx only — but for pure dark & white, skip this.

9) Export
- When satisfied, export as PNG for transparency (File > Export As), or as JPG if flattened background and posterized effect is desired.