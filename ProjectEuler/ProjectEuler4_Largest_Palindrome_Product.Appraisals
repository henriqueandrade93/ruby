#!/bin/ruby

def is_palin?(mul)
  mul.to_s == mul.to_s.reverse
end

def largest_palin(n, min = 100, max = 999)
  palin = 0
  range = min..max
  range.each do |x|
    x.upto(max).each do |y|
      mul = x*y
      break if mul > n
      palin = mul if is_palin?(mul) && mul > palin
    end
  end
  return palin
end


t = gets.strip.to_i
for a0 in (0..t-1)
  n = gets.strip.to_i

  puts largest_palin(n)
end