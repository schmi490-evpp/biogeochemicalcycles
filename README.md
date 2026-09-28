# Element Pathways

A static, self-contained classroom game. Students choose carbon, nitrogen, or phosphorus, then work through five shuffled clues. They choose a chemical form, place it in a reservoir on the supplied landscape, see the process, and answer a short application question. Click-to-place works on touchscreens and keyboards; desktop users can also drag a form to a location.

## Run locally

Open `index.html` in a browser. No build, account, package manager, or external service is required. For a local server, run `python3 -m http.server 8000` in this folder, then visit `http://localhost:8000`.

## Publish with GitHub Pages

1. Create a repository and upload **the contents of this folder** to the repository root (`index.html`, `styles.css`, `game.js`, and `assets/`).
2. In the repository's **Settings → Pages**, select **Deploy from a branch**, choose your branch and the **/(root)** folder, then save.
3. Open the HTTPS Pages URL GitHub displays and check the images and click targets on a phone or laptop.

If you upload the enclosing `element-cycle-game` folder instead, set that folder as your publishing source or move its contents to the root. The asset URLs are relative, so they work on project Pages URLs such as `https://USERNAME.github.io/REPOSITORY/`.

## Add to Canvas

Put the Pages URL on a Canvas Page as a normal link first. If your institution permits external iframes in the Rich Content Editor, you can try the HTML editor with:

```html
<iframe src="https://USERNAME.github.io/REPOSITORY/" title="Element Pathways game" width="100%" height="900" loading="lazy"></iframe>
```

Replace the URL with your actual HTTPS Pages URL. Preview the Canvas page as a student. Some Canvas configurations restrict iframes; in that case, use the direct link. The game does not send scores to Canvas or store student information. If you want a graded submission, ask students to submit a short reflection or screenshot through a separate Canvas assignment.

## Edit the content

All cycle data, correct answers, bonus questions, and image hotspot positions are at the top of `game.js`. Positions use `x` and `y` percentages relative to the image (0–100). Images are in `assets/`.

The three backgrounds are the images supplied for this activity by the instructor. Keep their attribution and reuse permissions in mind if publishing the repository publicly.
