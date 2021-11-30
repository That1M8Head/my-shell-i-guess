#include <stdio.h>
#include <string.h>

int main()
{
    /* Startup message */
    puts("My Shell I Guess by Arsalan Kazmi");
    puts("Type 'help' for help, 'commands' for a command list or 'licence' for licence info.");
    /* Prompt */
    char cmd[100] = "";
    while(1) {
	/* Prompt */
	printf("¬> ");
	fgets(cmd, 100, stdin);
	cmd[strcspn(cmd, "\n")] = 0;
	/* Command handlers */
	if (!strcmp(cmd, "help")) {
	    puts("My Shell I Guess is a thing I made when I was bored and wanted to try making something only using Emacs.");
	    puts("If you find My Shell I Guess useful... why?");
	}
	if (!strcmp(cmd, "licence") || !strcmp(cmd, "license")) {
	    puts("My Shell I Guess is licensed under the GNU General Public Licence, version 3.\n"
		 "You can get a copy of the licence at <https://gnu.org/licenses/gpl-3.0.html>.");
	}
	if (!strcmp(cmd, "commands")) {
	    puts("Command list\n"
	         "------------\n"
	         "help     - Show help.\n"
	         "licence  - Show licence information.\n"
	         "commands - The command you just typed.\n"
	         "exit     - Exit the program.");
	}
	if (!strcmp(cmd, "exit") || !strcmp(cmd, "quit")) {
	    break;
	}
    }
}
