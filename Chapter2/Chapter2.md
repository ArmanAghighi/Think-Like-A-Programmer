2.3:
As explaind to solve these kind of problem we need to find a pattern that stars (or hashtags) are printed using for loops.
in this question something like the shape below is going to be printed.

   *           *
    **       **
     ***   ***
      *******
      *******
     ***   ***
    **       **
   *           *
  as I found out there might be a pettern for this shape when you devide it to two up and down pieces.
  on the other hand it needs 4 for loops for each up and down piece to print 
  1.Left side spaces
  2.Left side *
  3.Middle spaces
  4.Right side stars

  To find the pattern we must write each row * or space and find out how it grows 
  for example for i = 0 of middle space there are 8 space and it reduce by the number 2 for each row so the formulla is (-4 * Row) + 12 I did this for all lines and the code below is the resault:

namespace Excersices
{
    public static class Shape4
    {
        public static void Draw()
        {
            int maxCount = 4;
            for (int Row = 0; Row < maxCount; Row++)
            {
                for (int LeftSpace = 0; LeftSpace < Row; LeftSpace++)
                {
                    Console.Write(" ");
                }
                for (int LeftSharp = 0; LeftSharp < Row + 1; LeftSharp++)
                {
                    Console.Write("#");
                }
                for (int BetweenSpace = 0; BetweenSpace < (-4 * Row) + 12; BetweenSpace++)
                {
                    Console.Write(" ");
                }
                for (int RightSharp = 0; RightSharp < Row + 1; RightSharp++)
                {
                    Console.Write("#");
                }
                Console.WriteLine();
            }
            for (int Row = 0; Row < maxCount; Row++)
            {
                for (int LeftSpace = 0; LeftSpace < -Row + 3; LeftSpace++)
                {
                    Console.Write(" ");
                }
                for (int LeftSharp = 0; LeftSharp < -Row + 4; LeftSharp++)
                {
                    Console.Write("#");
                }
                for (int BetweenSpace = 0; BetweenSpace < 4 * Row; BetweenSpace++)
                {
                    Console.Write(" ");
                }
                for (int RightSharp = 0; RightSharp < -Row + 4; RightSharp++)
                {
                    Console.Write("#");
                }
                Console.WriteLine();
            }
        }
    }
}
