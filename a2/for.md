var obj = [
          { person: "Name 1", age: "2", company: "GUVI" },
          { person: "Name 2", age: "5", company: "GUVI geek" },
          { person: "Name 3", age: "8", company: "GUVI geek network" },
        ];\
for(let i = 0;i<obj.length;i++)
{
     for(let j in obj[i])
     {
         console.log(j + ':' + obj[i][j]);
     }
}\
for(let i in obj)
{
    for(let j in obj[i])
     console.log(j + ":" + obj[i][j]);
}\
for(let i = 0;i<obj.length;i++)
{
  for (const [key, value] of Object.entries(obj[i]))
    console.log(`${key}: ${value}`);
}\
for(let i = 0;i<obj.length;i++)
{
    Object.entries(obj[i]).forEach(([key, value]) => {
     console.log(`${key}: ${value}`)
    });
}
