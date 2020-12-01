 static void Main(string[] args)
        {
            bool mode = true;
            int X = 0, Y = 0;
            char[,] array = new char[15, 45];
            Console.WriteLine("Mode is active");
            Thread.Sleep(1000);
            Console.Clear();
            ConsoleKeyInfo keyInfo = new ConsoleKeyInfo();
            Operation operation = new Operation();
            while (true)
            {
                keyInfo = Console.ReadKey();
                
                if (keyInfo.Key == ConsoleKey.Spacebar)
                {
                    if (mode) mode = false;
                    else mode = true;
                }
               
                if (!mode)
                {
                   
                    Console.WriteLine("Mode is passive");
                    Thread.Sleep(1000);
                    Console.Clear();
                    if (FindKey(keyInfo) == 1)
                    {

                        Y++;
                        operation.DownOP(array, X, Y);


                    }
                    else if (FindKey(keyInfo) == 2)
                    {
                        Y--;
                        char[,] array1 = operation.UpOP(array, X, Y);
                    }
                    else if (FindKey(keyInfo) == 3)
                    {
                        X--;
                        operation.LeftOP(array, X, Y);
                    }
                    else if (FindKey(keyInfo) == 4)
                    {
                        X++;
                        operation.RightOP(array, X, Y);
                    }
                    else if (keyInfo.Key == ConsoleKey.Escape)
                        break;
                    else if(keyInfo.Key!=ConsoleKey.Spacebar)
                    {
                        Console.WriteLine("Wrong Key!!!");
                    }
                }
                else
                {
                   
                    Console.WriteLine("Mode is active");
                    Thread.Sleep(1000);
                    Console.Clear();
                    if (FindKey(keyInfo) == 1)
                    {
                       
                        Y++;
                        char[,] array1 = operation.DownOP(array, X, Y);
                        for (int i = 0; i < 15; i++)
                        {
                            for (int j = 0; j < 45; j++)
                            {
                                Console.Write(array1[i, j]);
                            }
                            Console.WriteLine();
                        }

                    }
                    else if (FindKey(keyInfo) == 2)
                    {
                        
                        Y--;
                        char[,] array1 = operation.UpOP(array, X, Y);
                        for (int i = 0; i < 15; i++)
                        {
                            for (int j = 0; j < 45; j++)
                            {
                                Console.Write(array1[i, j]);
                            }
                            Console.WriteLine();
                        }


                    }
                    else if (FindKey(keyInfo) == 3)
                    {
                       
                        X--;
                        char[,] array1 = operation.LeftOP(array, X, Y);
                        for (int i = 0; i < 15; i++)
                        {
                            for (int j = 0; j < 45; j++)
                            {
                                Console.Write(array1[i, j]);
                            }
                            Console.WriteLine();
                        }


                    }
                    else if (FindKey(keyInfo) == 4)
                    {
                       
                        X++;
                        char[,] array1 = operation.RightOP(array, X, Y);
                        for (int i = 0; i < 15; i++)
                        {
                            for (int j = 0; j < 45; j++)
                            {
                                Console.Write(array1[i, j]);
                            }
                            Console.WriteLine();
                        }

                    }
                    else if (keyInfo.Key == ConsoleKey.Escape)
                        break;
                    else if(keyInfo.Key!=ConsoleKey.Spacebar)
                    {
                        Console.WriteLine("Wrong Key!!!");
                    }
                }




            }
            for (int i = 0; i < 15; i++)
            {
                for (int j = 0; j < 45; j++)
                {
                    Console.Write(array[i, j]);
                }
                Console.WriteLine();
            }
            Console.WriteLine("------> Program is finished <------(Please , press to ENTER.)");
            Console.ReadKey();
        }
