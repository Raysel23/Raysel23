#include "iostream.h"
#include "stdio.h"
#include "alloc.h"
#include "conio.h"

//Defining structure of the node

struct Double {

   int info;
   struct Double *next;
   struct Double *previous;
   };

//Defining class doubly linked-list

class doubly_link {

   public:
      int num;
      Double start, *temp;
   public:
      void Doubly_Create(Double *);
      void Doubly_Insert(Double *);
      void Doubly_Delete(Double *);
      void display(Double *);
      };

      //Function definition for doubly_create()

  void doubly_link::Doubly_Create(Double *node) {

     start.next = NULL;
     start.previous = NULL;

     //Start is the first node in the Doubly linked-list

     node= &start;
     num = 0;
     cout next = (Double *)malloc (sizeof(Double));

     //Point the previous link of next node to start node

	node->next->previous = node;

     //The next node becomes the start node now

	node = node->next;

     //Read data value for the node

	cout > node->info;

     //The Next Pointer of the node points to NULL

	node->next = NULL;

	cout previous->next = node->next;
	  node->next->previous = node->previous;
	  free(node);
	  }
	}

	//Function definition for Doubly_Insert()

	void doubly_link::Doubly_Insert(Double *node) {

	   temp = (Double*)malloc(sizeof(Double));

	   cout > temp->info;

	   node = start.next;

	   if(node == NULL) {

	      cout next = node;

	   //The temp node previous points to
	   //start node next (node->previous)

	      temp->previous = node->previous;

	   //Start node (node->previous) next pointer
	   //points to new temp node

	      node->previous->next = temp;
	      }
	   }

	  //Function definition for display()

	  void doubly_link::display(Double *node) {

	      node = start.next;

	      do {
		 cout ";
		 cout info;
		 node = node->next;
		 }while(node != NULL);

		 getch();
	      }

	      //MAIN PROGRAM STARTS HERE

	      void main() {

		 doubly_link dlinked_list;
		 int br;

		 clrscr();

		 cout > br;

		 while(br != 0) {

		   switch(br) {

		    case 1:

		     Double *node = (Double *)malloc(sizeof(Double));
		     dlinked_list.Doubly_Create(node);
		     break;

		    case 2:
		     cout > br;
	      }
	  }
