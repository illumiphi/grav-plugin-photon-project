% name: Project
% def: post_date=$(date +%m/%d/%Y)
% def: author='/phi'
% def: start_dt=$(date +%m/%d/%Y)
% def: end_dt=$(date +%m/%d/%Y)
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
        - project
    tag: 
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


