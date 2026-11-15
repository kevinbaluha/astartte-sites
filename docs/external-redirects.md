# External Links and Old Path Redirects

This document lists key external references (from indexed Wix archives, directories, old newsletters, about pages, etc.) and how old paths on asttartedeva.com are resolved via 301 redirects in `_redirects`.

All redirects are on the `seo-review-oct2026` branch (PR #1) and will be live after merge to main.

## Old Paths Referenced in External Sources → Redirect Targets

These prevent 404s when people or search engines follow old links from external indexed content.

### Coaching / Intimacy / Tantra cluster
- /coaching, /services/coaching, /services/coaching/ → /services/intimacy-coaching/
- /intimacy, /intimacy-coaching → /services/intimacy-coaching/
- /couples-coaching → /services/intimacy-coaching/
- /tantra-coaching → /services/intimacy-coaching/
- /tantra → /services/intimacy-coaching/
- /grief-coaching → /services/intimacy-coaching/

### Energy / Reiki cluster
- /reiki, /services/reiki → /services/reiki-traditions/
- /reiki-and-energy-healing, /services/reiki-and-energy-healing → /services/reiki-and-energy-healing/
- /private-healing → /services/reiki-and-energy-healing/
- /energy-healing-sessions → /services/reiki-and-energy-healing/
- /chakra-balancing → /services/reiki-and-energy-healing/
- /past-life-healing → /services/reiki-and-energy-healing/
- /shamanic → /services/reiki-and-energy-healing/

### Massage / Bodywork
- /massage, /massage-therapy → /services/massage-therapy/

### Somatic
- /somatic-stress-release, /somatic-stress-release-therapy → /services/somatic-stress-release/

### Breathwork
- /breathwork → /services/breathwork/

### Yoga / Meditation
- /yoga-and-meditation, /services/yoga-and-meditation, /yoga → /services/private-yoga-sessions/

### Sound
- /sound, /sound-healing, /about-4 → /services/sound-healing/

### Tarot / Readings
- /tarot, /tarot-astrology-readings → /services/tarot-astrology-readings/

### Other
- /eft, /eft-tapping → /services/eft/
- /holistic-health → /services/holistic-health/
- /plant-medicine-psychedelic-integration, /plant-medicine → /services/breathwork/
- /cacao, /cacao-ceremonies → /services/cacao-ceremonies/
- /additional-energy-practices → /services/additional-energy-practices/
- /spiritual-holistic-form → /contact/

### Legacy / Broad
- /post/* → /blog/ (301)
- /blog/* → /blog/ (200 - keep as is for blog index)

## External Sites That List Services (Separate from our domain redirects)

These are still indexed and list services under old or alternate descriptions. They are not on asttartedeva.com paths, so our redirects do not affect them directly. Our canonical site can outrank them over time with better content and signals.

- https://asttartedeva.wixsite.com/centerforhealingarts  
  Lists: Reiki & Energy Healing (Chakra, IET, Igili, etc.), Massage Therapy (Acupressure, Thai, Shiatsu, Shamanic), Somatic Stress Release, Breathwork, Yoga & Meditation, Intimacy/Attachment & Trauma-Informed Coaching, Tarot & Intuitive Readings, Holistic Health and Heart-Opening Healing, Sound Healing.

- https://asttartedeva.wixsite.com/asttartedeva  
  Lists: Somatic Healing, Psychedelic Integration, Breathwork, Conscious Relationship Work, Sound Healing, Plant Medicine Therapy, Retreats (Breathwork, Yoga, Meditation, Somatic, Sound), Heart Opening Healing, One on One Sessions, Integration Sessions.

- https://fairiesinamerica.com/supernatural-healings/energy-healer-asttarte-deva/  
  Lists: Channeled Life Coach, Guided Meditation Sessions, Soul Aura Readings and Healing, Sound Healing, Pendulum Readings, Ascension Prayer Treatment, Women’s Coaching, Reiki Intuitive Energy Healing.

- https://about.me/asttarte  
  Lists: Somatic Healing, Psychedelic Integration Guide, Breathwork Facilitator, Shamanic Facilitator, Holistic Wellness Guide (over 25 years experience).

- Yelp (Asttarte Deva Healing Wellness Center, Philadelphia): breathwork, meditation, reiki, intuitive energy healing, somatic stress release therapy, sound healing, tantra yoga holistic health & wellness, trauma recovery, relationship and couples coaching.

- Alignable (Bala Cynwyd): Tantra & Shamanic Soul Healing & Coaching, Yoga, Reiki, Breathwork, Meditation, Shadow Bodywork & Couples Coaching, Private Sessions, Retreats.

- Various Mailchimp/newsletters (old): Direct links to paths like /breathwork, /plant-medicine-psychedelic-integration, /somatic-stress-release-therapy, /sound-healing, /grief-coaching, /eft-tapping, /energy-healing-sessions, /chakra-balancing, /past-life-healing, /couples-coaching, /tantra-coaching, /reiki, etc. (now covered by redirects above).

- YouTube channel descriptions and videos: Attachment & intimacy healing, Conscious relationships, Psychedelic preparation & integration, Embodiment & somatic awareness, Meditation & breathwork, Emotional healing & grief, etc.

- Other directories (Nextdoor, MapQuest, etc.): Similar holistic, breathwork, reiki, somatic, sound, coaching listings.

## Notes
- Redirects use 301 (permanent) to pass link equity to the target pages.
- Targets are the closest current, optimized service pages.
- After PR merge and publish, test a few old paths (e.g. curl -I https://www.asttartedeva.com/plant-medicine-psychedelic-integration).
- Submit sitemap for indexing after merge to help search engines pick up the current structure.
- External Wix and third-party listings will continue until updated by their owners or outranked.

Last updated on seo-review-oct2026 branch.