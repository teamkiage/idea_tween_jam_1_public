# idea_tween_jam_1_public

-- primeDad
r,tm,sc,sz,c=63,0,{},128,0
_sqrt=function(n)
 if sc[n] then return sc[n] end
 sc[n] =  sqrt(n)
 return sc[n]
end
::_::
 cls()
 cursor(47,60)  
-- ?"\#9kiage"
 ?"\^wkiage"
--?"\^wmixi \n"
?"\^w \^t  😐\n"

 for y=-r,r,3 do for x=-r,r,3 do
  local z = cos(_sqrt(x*x+y*y*2)/40-tm)*6/c
  local dx,dy=r+x,r+y-z-sz/8
  if dx>0 and dy>0 and dx<sz and dy<sz then
   -- pset(dx-2,dy-1, (flr(t()+1*2%10)) )
   pset(dx-2,dy-1, dx%2==0 and rnd({8,9}) or 10)   
  end
 end end
 flip()
 tm=tm+ 2/r
c=(c>=12 and 0 or c)c+=0.01
goto _
