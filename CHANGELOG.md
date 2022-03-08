# Changelog  
All notable changes to this project will be documented in this file.  

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).  

## [Unreleased]  

## [0.9.1] - 2022-03-08  
### Added  
- Additional zines  
- Additional CSS styles, particularly for "details"/"summary" interactive elements on `01-sift-moves.md` page  
    - Added styles to `main.scss`  
    - Added `<div markdown="1" class="details-wrapper">` to appropriate sections in SIFT moves  

### Changed
- Restructured underlying files to make search function work correctly (lunr will index contents of blog posts or pages in collections, but not content of regular pages in `_pages` folder); this also automatically added "Previous / Next" buttons at the bottom of pages in `_content-pages` / `content-pages` collection  
    - Created folder called `_content-pages`  
    - Added `content-pages` collection info to `_config.yml`  
    - Renamed the pages in `_content-pages` to create an ordered structure for "Previous / Next" button pagination (order is alphabetical, so it's controlled by prefixing the page names with numbers, i.e. `01-sift-moves.md` instead of the former name, `sift-moves.md`)  
- Reworded 5Ps section on `10-about.md`  
- Reworded some parts of `01-sift-moves.md` and made "Don't Stress, SIFT" a heading  
- Reordered navigation so that "About" page comes last  
- Reworded `home.md` and added final paragraph with links beyond SIFT  
- Commented out unused lines in `navigation.yml`  
- Updated copyright span of years, aka `lifespan` in `_config.yml`  
- Updated contributions on `10-about.md`  

## [0.9.0] - 2021-03-04  
### Added  
- `CHANGELOG.md` file  
- "Version Information" section to `About.md` page, with 5Ps  

### Changed  
- Reworded `Home.md` slightly, including addition of NY Times article link  
- Reworded license information on `About.md` and `zines.md` to increase specificity  
- Reworded license information to increase specificity in footer (via `_includes/footer.html`)  