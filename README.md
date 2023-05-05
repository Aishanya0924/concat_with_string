# concat_with_string
```
#include <stdio.h>
#include <string.h>
int main()
{
        char cat[100];

        // Copy the first string into
        // the variable
        strcpy(cat, "Aishanya");

        // Concatenate this string
        // to the end of the first one
        strcat(cat, " Manoj");

        // Display the concatenated strings
        printf("%s\n", cat);

        return 0;
}
```

```
#include <stdio.h>

int main()
{

        // Get the two Strings to be concatenated
        char begin[100] = "Aishanya ", last[100] = "Manoj";

        // Declare a new Strings
        // to store the concatenated String
        char end[100];

        int i = 0, j = 0;

        printf("\nFirst string: %s", begin);
        printf("\nSecond string: %s", last);

        // Insert the first string
        // in the new string
        while (begin[i] != '\0') {
                end[j] = begin[i];
                i++;
                j++;
        }

        // Insert the second string
        // in the new string
        i = 0;
        while (last[i] != '\0') {
                end[j] = last[i];
                i++;
                j++;
        }
        end[j] = '\0';

        // Print the concatenated string
        printf("\nConcatenated string: %s\n", end);

        return 0;
}
```
