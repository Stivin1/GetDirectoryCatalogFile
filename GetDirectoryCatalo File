public static class Program
{
        public static void Main(string[] args)
        {
            DirectoryInfo getdirectory = new DirectoryInfo(@"D:\");
            Direct(getdirectory.FullName);
        }

        public static void Direct(string DirectoryFullName)
        {
            foreach (var list in Directory.GetDirectories(DirectoryFullName))
            {
                Console.WriteLine(list);

                var fileInfos = Directory.GetFiles(list);

                foreach(var list1 in fileInfos)
                {
                    Console.WriteLine(list1);
                }
                
                Direct(list);
            }
        }
}
