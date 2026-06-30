**GitHub Repo Description** (one-liner for the About field):

> Project page for M3Grounder — mask-based multi-span & multi-granular grounding for Document QA. CVPR 2026.

---

**README.md:**

```markdown
# M3Grounder — Project Page

**[CVPR 2026]** Official project page for  
**M3Grounder: Mask-Based Multi-Span and Multi-Granular Grounding for Document QA**  
*BharatGen & IIIT Hyderabad*

🔗 [Paper](https://openaccess.thecvf.com/content/CVPR2026/papers/Venna_M3Grounder_Mask-Based_Multi-Span_and_Multi-Granular_Grounding_for_Document_QA_CVPR_2026_paper.pdf) · [HF Space](https://huggingface.co/spaces/m3grounder/m3grounder) · [Code](https://github.com/m3grounder/m3grounder) · [Poster](https://cvpr.thecvf.com/media/PosterPDFs/CVPR%202026/38567.png)

---

## What is M3Grounder?

M3Grounder grounds document QA answers at pixel level — not just bounding boxes. It autoregressively generates answer text interleaved with `[GROUND]` tokens that link each answer span to its evidence region on the page, at **phrase, line, and block** granularity.

Key ideas:
- **Mask-based grounding** — fine-grained segmentation instead of coarse boxes
- **Multi-span** — one answer can cite multiple evidence regions
- **Multi-granular** — phrase ⊂ line ⊂ block, enforced by an enclosure loss
- **Bleed-suppression loss** — prevents masks from spilling into irrelevant regions

---

## This Repo

Static project page built with plain HTML/CSS/JS. Includes an interactive demo showcasing multi-span, multi-granular grounding across Finance, Legal, and Transcript documents.

```
index.html          # entire site (single file)
static/
  images/           # logos, teaser, document images
```

To run locally:
```bash
python -m http.server 8000
# open http://localhost:8000
```

---

## Citation

```bibtex
@inproceedings{venna2026m3grounder,
  title     = {M3Grounder: Mask-Based Multi-Span and Multi-Granular Grounding for Document QA},
  author    = {Venna, Venkata Kesav and Gunda, Sai Madhusudan and Jinka, Jyothi Swaroopa
               and Rachakonda, Hrithik Sagar and Srinivasan, Anirudh and Sarvadevabhatla, Ravi Kiran},
  booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages     = {23685--23695},
  year      = {2026}
}
```
```
