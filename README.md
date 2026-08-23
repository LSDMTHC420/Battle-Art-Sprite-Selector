I built a voxel-free sprite selector as a separate graphics mod, so it can sit alongside any of the Kanto + Johto Dex variants without duplicating them.

Download Battle Art Sprite Selector v1.0.0

It adds one compact ART option with 19 choices:

DFLT / RB / GRN / YEL / GLD / SLVR / CRYS / RS / EMRD / FRLG / DP / PLAT / HGSS / BW / PIN / PIRS / TRZ / MD1 / MD2

The important part is exactly what you requested: every selection is a per-sprite overlay. If HGSS only has a sprite for a particular Pokémon or trainer, that one changes; anything missing falls straight back to the currently active default. With our Kanto/Johto Dex mod, that means missing Pokémon retain the existing animated sprites rather than going blank or borrowing something incorrect.

I also wired in dedicated shiny art where the pack provides it, shared back-sprite sets where appropriate, trainer art tied to the same ART selection, and automatic sizing for the wildly different sprite resolutions. DFLT completely yields back to our existing animated sprite implementation.

The original Battle Art Voxel Fork is intentionally marked as conflicting, since this replaces its art-selection concept without loading any voxel renderer/camera/world code. The final archive is about 21 MB, ZIP integrity passed, and the build includes a coverage QA report for every style.
