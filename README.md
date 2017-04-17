array1 =[11,12,13]
array2 =[21,22,23]
array3 =[31,32,33]
array0 = [array1, array2, array3]

array0.each do |x| puts "#{x}\n" 
end
puts "place your krestik"
krestik = gets.chomp.to_i

array0.collect! do |i| 
   if i.include?(krestik) 
     i[i.index(krestik)] = 'x'; i 
   else
     i
   end
 
end 

array0.each do |x| puts "#{x}\n" 
end

if array2[1] != 'x'
array2[1] = '0'
else 
puts 'bad'
end
puts '   '

array0.each do |x| puts "#{x}\n" 
end

puts "place your next krestik"
krestik2 = gets.chomp.to_i


array0.collect! do |i| 
   if i.include?(krestik2) 
     i[i.index(krestik2)] = 'x'; i 
   else
     i
   end
 
end 

array0.each do |x| puts "#{x}\n" 
end
puts ' '


if array2[0] != 'x'
array2[0] = '0'
else 
puts 'bad'
end
puts '   '

array0.each do |x| puts "#{x}\n" 
end

puts "place your next krestik"
krestik3 = gets.chomp.to_i


array0.collect! do |i| 
   if i.include?(krestik3) 
     i[i.index(krestik3)] = 'x'; i 
   else
     i
   end
 
end 

array0.each do |x| puts "#{x}\n" 
end
puts 'YOU WIN'
