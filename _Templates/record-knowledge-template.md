---
tags:
<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(`${title}`);
  } 
%>
---
# :LiList: Table of Contents
---



# Topic Header
---
### <u>Key Terms & Definitions</u>
- Key Terms: Definitions of the key terms related to this topic.

### <u>Key Concepts</u>
- Explanation of the key concepts of this topic.


# :LiListFilter: Highlights
---
### <u>Key Takeaways</u>
- Key takeaways from this note.

### <u>Important Dates</u>
- List of important dates (if applicable).

### <u>Formulas & Equations</u>
- List of important formulas (if applicable).

### <u>Graphs & Charts</u>
- List of important graphs (if applicable).