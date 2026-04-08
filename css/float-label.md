---
eleventyNavigation:
  parent: css
  key: <i class="fa-solid fa-picture-in-picture fa-flip-both"></i> Label
  order: 2
title: <a href="/css/">CSS</a> Float Label <sup><img src="https://img.shields.io/github/v/release/anyblades/float-label-css?label=&color=black&include_prereleases"></sup>
eleventyComputed:
  summary: |-
    {% liquid
      assign _ = 'https://raw.githubusercontent.com/anyblades/float-label-css/refs/heads/master/README.md'
      # assign _ = '../../float-label-css/README.md'
      echo _ | fetch | section: 'summary'
    %}
    https://github.com/anyblades/float-label-css  
    from https://github.com/anyblades/blades
includes:
  - section: intro
    path: https://raw.githubusercontent.com/anyblades/float-label-css/refs/heads/master/README.md
    # path: ../../float-label-css/README.md
  - text: |-
      ## Demo

      Drop-in support for **Pico**'s https://picocss.com/docs/forms :

      <article>
        <!-- Sample markup from https://codepen.io/anton-staroverov/pen/JRLaKw -->
        <form>
          <fieldset>
            <legend>Demo form</legend>
            <label><span>Name</span>
              <input placeholder="First Last">
            </label>
            <label><span>Bio</span>
              <textarea placeholder="Tell your story..."></textarea>
            </label>
            <label><span>Cuisine</span>
              <select>
                <option selected disabled>Select...</option>
                <option>Italian</option>
                <option>Japanese</option>
                <option>Indian</option>
                <option>Thai</option>
                <option>French</option>
              </select>
            </label>
            <button type="button">Sign up</button>
            <button type="reset">↺</button>
          </fieldset>
        </form>
      </article>

      More examples:
  - section: docs-demo-install
    path: https://raw.githubusercontent.com/anyblades/float-label-css/refs/heads/master/README.md
    # path: ../../float-label-css/README.md
  - text: <details><summary role="button" class="outline">Install Blades CSS Kit</summary>
  - section: install
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/README.md
  - text: </details>
  - text: |-
      ---
      ## How it works {#how}
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/float-label.core.css
---
