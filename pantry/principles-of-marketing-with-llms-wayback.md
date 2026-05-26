# Wayback Image Prompts — Principles of Marketing with LLMs

Text-to-image prompts generated from the AI Wayback Machine sections in `chapters/`.
Each prompt is anchored to the historical figure named in the chapter section.

```python
principles_of_marketing_with_llms = [
    # chapters/01-setting-the-stage.md — Philip Kotler
    "Philip Kotler (circa 1967, American marketing scholar) - middle-aged man in suit, marketing management notes nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/02-marketing-and-customer-value.md — Theodore Levitt
    "Theodore Levitt (circa 1960, American marketing scholar) - middle-aged man in suit, marketing myopia notes nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/03-strategic-planning-in-marketing.md — Igor Ansoff
    "Igor Ansoff (circa 1965, Russian-American strategist) - middle-aged man in suit, strategy matrix nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/04-understanding-the-marketplace.md — Wroe Alderson
    "Wroe Alderson (circa 1957, American marketing theorist) - middle-aged man in suit, market behavior notes nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/05-consumer-markets-and-purchasing-behavior.md — Ernest Dichter
    "Ernest Dichter (circa 1950, Austrian-American psychologist and marketing researcher) - middle-aged man in suit, motivation research notes nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/06-business-markets-and-purchasing-behavior.md — Frederick Webster
    "Frederick Webster (circa 1991, American marketing scholar) - middle-aged man in suit, industrial marketing notes nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/07-market-segmentation-targeting-and-positioning.md — Wendell Smith
    "Wendell Smith (circa 1956, American marketing scholar) - middle-aged man in suit, segmentation diagrams nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/08-marketing-research-and-market-intelligence.md — George Gallup
    "George Gallup (circa 1935, American polling pioneer) - middle-aged man in suit, survey forms nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/09-marketing-in-a-global-environment.md — C. K. Prahalad
    "C. K. Prahalad (circa 1990, Indian management scholar) - South Asian man with glasses, global strategy notes nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/10-marketing-in-a-diverse-marketplace.md — Tom Burrell
    "Tom Burrell (circa 1975, African American advertising executive) - Black man in suit, multicultural advertising boards nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/11-product-promotion-price-and-place.md — E. Jerome McCarthy
    "E. Jerome McCarthy (circa 1960, American marketing professor) - middle-aged man in suit, 4Ps notes nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/12-products-consumer-offerings.md — David Ogilvy
    "David Ogilvy (circa 1963, British advertising executive) - middle-aged man in suit, advertising copy boards nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/13-maintaining-a-competitive-edge-with-new-offerings.md — Clayton Christensen
    "Clayton Christensen (circa 1997, American business scholar) - middle-aged man in suit, disruptive innovation diagrams nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/14-services-the-intangible-product.md — Christopher Lovelock
    "Christopher Lovelock (circa 1990, British services marketing scholar) - middle-aged man in suit, services blueprint notes nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/15-pricing-products-and-services.md — Hermann Simon
    "Hermann Simon (circa 1990, German pricing strategist) - middle-aged man in suit, pricing curves nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/16-integrated-marketing-communications.md — Don Schultz
    "Don Schultz (circa 1993, American marketing communications scholar) - middle-aged man in suit, integrated communications diagrams nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/17-the-promotion-mix-advertising-and-public-relations.md — Edward Bernays
    "Edward Bernays (circa 1928, Austrian-American public relations pioneer) - middle-aged man in suit, public relations campaign papers nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/18-the-promotion-mix-personal-selling-and-sales-promotion.md — Mary Kay Ash
    "Mary Kay Ash (circa 1965, American entrepreneur) - woman with styled hair, pink business suit, cosmetics sales materials nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/19-direct-online-social-media-and-mobile-marketing.md — Lester Wunderman
    "Lester Wunderman (circa 1967, American direct marketing pioneer) - middle-aged man in suit, direct mail campaign materials nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/20-distribution-delivering-customer-value.md — Louis Bucklin
    "Louis Bucklin (circa 1966, American marketing channels scholar) - middle-aged man in suit, distribution channel diagrams nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/21-retailing-and-wholesaling.md — Stanley Marcus
    "Stanley Marcus (circa 1955, American retailer) - middle-aged man in suit, department store merchandising notes nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
    # chapters/22-sustainable-marketing-the-new-paradigm.md — Donella Meadows
    "Donella Meadows (circa 1972, American systems scientist) - young woman with long dark hair, sustainability systems diagrams nearby, historically plausible editorial portrait, face-centered composition, period-appropriate clothing and workspace, accurate to known public portraits or photographs when available, no text, no watermark",
]
```
