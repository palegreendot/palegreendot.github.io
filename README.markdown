# Seattle Rationality Reading Group Notes Site

## Adding New Notes
1. In the `_posts` directory, create a new file with the following name: `<date>-rrg-reading-notes.markdown`
    * Dates are formatted YYYY-MM-DD, and should be the date of the meeting, not the date the notes were authored
    * Example filename: 2018-02-19-rrg-reading-notes.markdown
2. The new file should have the following [YAML front matter](https://jekyllrb.com/docs/frontmatter/)
   ```yaml
    ---
    layout: post
    title: "<meeting_date>"
    date: <publication_date_time> <timezone>
    categories: rrg_notes
    ---
    ```
        * Meeting date should be of the format `<month> <day> <year> RRG Notes`
            * Example: `February 19 2017 RRG Notes`
        * Publication date-time should be the time you started writing the notes - needs to be in the past, otherwise Jekyll will not actually publish the notes
            * Example: `2018-02-19 08:00`
        * Timezone is the UTC offset of the timezone you're publishing from, usually -0800/-0700 (if publishing from PST/PDT, respectively)
3. Notes format:
    * Each article should have a 2nd level heading `##` that is a link to the article
    * Write notes as an outline, not as prose
