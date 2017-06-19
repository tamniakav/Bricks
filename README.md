using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Bricks
{
    class Program
    {
        static void Main(string[] args)
        {
            int bricks = int.Parse(Console.ReadLine());
            int workers = int.Parse(Console.ReadLine());
            int capacity = int.Parse(Console.ReadLine());

            int howManyBricks = workers * capacity;
            int courses = (bricks / howManyBricks);
            int f = courses * howManyBricks;

            if (f == bricks)
            {
                Console.WriteLine(courses);
            }
            else
            {
                Console.WriteLine(courses + 1);
            }
        }
    }
}

