# Pre-filled support and wrong-answer emails

## Choice

Add two buttons under "Getting help" on the support page:

- **Email support**: opens the visitor's email app with the subject "Spinola support" and a short template asking what they were doing, what happened, which mode they were in, and their phone or tablet model.
- **Report a wrong answer**: opens an email with the subject "Spinola: wrong answer" and asks for the question text, the answer Spinola gave, the correct answer, and a source.

The "A question has the wrong answer" FAQ entry now links to the report button.

## Reasoning

The site is two static pages, and the support page's main job is getting useful reports to Noah. It already lists what a good report should include ("what you were doing, which mode you were in, and your phone or tablet model"; "with the question text"), but the email link was bare, so people had to remember that list on their own. Wrong-answer reports matter because "every question is meant to be a checkable public fact". Asking for a source makes those reports quicker to check.

`mailto:` links with `subject` and `body` parameters work without JavaScript or a build step, so the site keeps its "plain static HTML" approach. The buttons reuse the existing `--violet`/`--paper` colours, so they follow the dark-mode switch.

## Not done

- No contact form. It would need a server or a third-party service, and the privacy policy says there are none.
- No changes to the privacy policy.
