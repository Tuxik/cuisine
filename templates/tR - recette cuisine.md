<%*  const nomRecette = await tp.system.prompt("quel est le nom de la recette ?", "nom de la recette", false, false); await tp.file.rename(nomRecette); %>
## Ingredients 

<%* const nomListeCourse = "Liste de courses pour " + nomRecette; %>
![[<%* tR += ( await tp.file.create_new(tp.file.find_tfile("tR - liste de course recette"), nomListeCourse, false, app.vault.getAbstractFileByPath("liste de courses")) ).basename; %>]]
## Instructions

1.  <% tp.file.cursor(1) %>
## Notes



