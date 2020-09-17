% name: Project
% def: post_date=$(date +%m/%d/%Y)
% def: author='/home'
% def: start_dt=$(date +%Y-%m-%d)
% def: end_dt=$(date +%Y-%m-%d)
---
title: ${title}
subtitle: ${subtitle}
date: ${post_date}
author: ${author}
content:
    title: Actions
    items: '@self.children'
taxonomy:
    category: 
        - ${category}
    tag: 
        - ${tag}
show_gallery: false
data:
    project:
        '@type': Project
        startDate: ${start_dt}
        endDate: ${end_dt}
        location:
            '@type': Place
            name: ${place_name}
            address:
                streetAddress: ${place_street}
                addressLocality: ${place_city}
                addressRegion: ${place_state}
                postalCode: ${place_zip}
                addressCountry: ${place_country}
---

${summary}

===


